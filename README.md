# 코틀린 프로그래밍과 응용  
### 설계프로젝트 과제제안서  

- **과목명:** 코틀린 프로그래밍과 응용  
- **제출일자:** 2024년 12월 24일  
- **성명/학번:** 김동하 (22012231)  
- **소속 학과:** 디지털융합대학 컴퓨터학부, 정보통신공학전공  

---

## 과제 제안서  

### 과제명  
**Kotlin/JS 및 Spring Boot 기반 프로젝트 관리 시스템**  

### 과제기간  
**2024. 11. 31 (금) ~ 2025. 01. 31 (목)**  

---

## 1. 프로젝트 결과물 제목  
**ProManage**  
- 프로젝트 관리 시스템 **Manager.시점**

---

## 2. 주요 기능  
1. Kotlin Spring Boot 서버 통신 기반 로그인 및 프로젝트 정보 불러오기  
2. React, Kotlin/JS 기반 UI 디자인  
3. 여러 프로젝트를 관리하는 회사의 매니저를 위한 프로젝트 관리 시스템  

---

## 3. 팀 구성  
- 김동하 (22012231)

---

## 4. 세부 기능블럭도  

![세부 기능블럭도](images/기능블럭도.png)

---

## 5. 기능 순서도 (Sequence Diagram)  

### 로그인 기능 순서도  
![로그인 기능 순서도](images/로그인_순서도.png)

### 프로젝트 등록 기능 순서도  
![프로젝트 등록 순서도](images/프로젝트_등록_순서도.png)

---

## 6. 관련 Database 구성 및 Table 속성  

### 데이터베이스 ERD 구성도  
![ERD 구성도](images/ERD.png)

---

## 7. 주요 Kotlin 클래스 및 데이터 멤버  

- **Company_employee:**  
  `user_id`, `name`, `specialty`, `user_email`  

- **Project:**  
  `project_id`, `project_name`, `description`, `start`, `end`, `finish`  

- **ProjectMember:**  
  `user_id`, `project_id`, `task_name`, `task_description`  

---

## 8. 핵심 알고리즘  

1. **프로젝트 조회 및 관리 알고리즘**  
   - 프로젝트 상세 정보: 프로젝트에 대한 상세정보를 확인할 수 있는 알고리즘  
   - 프로젝트 관리: 프로젝트를 효과적으로 관리하기 위한 알고리즘  

2. **테스크 조회 및 관리 알고리즘**  
   - 테스크 관리: 직원의 ID로 담당하는 테스크를 등록하는 알고리즘  
   - 테스크 조회: 관리자가 화면에서 테스크를 선택해 더 자세한 테스크 정보를 볼 수 있는 알고리즘  

3. **직원 등록 및 관리 알고리즘**  
   - 직원 등록: 프로젝트에 참여할 직원을 등록하는 알고리즘  
   - 직원 삭제: 필요 없는 직원을 삭제하는 알고리즘  

---

## 9. 서버 구성  
### Server 구성  
![서버 구성도](images/서버구성.png)

---

## 10. Server Dependencies  

---

## 11. Client 화면 구성  

- **Main.page:**  
  유저 관리 또는 매니저 관리를 선택하는 페이지  

- **Member.page:**  
  유저를 관리하는 페이지  

- **Project.page:**  
  회사 유저의 목록을 삭제 및 추가 가능  

- **ProjectMember.page:**  
  프로젝트를 선택하면 상세 부분과 참여 멤버를 추가할 수 있는 페이지  

---

## 12. Docker Deployment  
- **Docker Sequence**  
  - Docker Hub push  
  - Docker 실행 및 작동  

---

## 13. MSA 구조  

### **Employee Service**  
- **역할:** 직원 정보를 관리하고 제공  
- **포함된 파일:**  
  - `model/Employee.kt`: 직원 엔티티  
  - `repository/EmployeeRepository`: 직원 데이터를 관리  
  - `service/EmployeeService`: 직원 관련 비즈니스 로직  
  - `controller/EmployeeController`: 직원 API 엔드포인트  

### **Project Service**  
- **역할:** 프로젝트 정보를 관리하고 제공  
- **포함된 파일:**  
  - `model/Project.kt`: 프로젝트 엔티티  
  - `repository/ProjectRepository`: 프로젝트 데이터를 관리  
  - `service/ProjectService`: 프로젝트 관련 비즈니스 로직  
  - `controller/ProjectController`: 프로젝트 API 엔드포인트  

### **Project Member Service**  
- **역할:** 프로젝트 멤버 정보를 관리하고 제공  
- **포함된 파일:**  
  - `model/ProjectMember.kt`: 프로젝트 멤버 엔티티  
  - `repository/ProjectMemberRepository`: 프로젝트 멤버 데이터를 관리  
  - `service/ProjectMemberService`: 프로젝트 멤버 관련 비즈니스 로직  
  - `controller/ProjectMemberController`: 프로젝트 멤버 API 엔드포인트  

### **Home Service**  
- **역할:** 초기 엔드포인트 제공  
- **포함된 파일:**  
  - `controller/HomeController`: 메인 엔드포인트를 제공  

---

### **이미지 추가 방법**
- `images/` 폴더에 이미지 파일 저장.
- Markdown에서 이미지 경로를 적절히 연결하세요.
- 예: `![이미지 설명](images/파일명.png)`

필요하면 추가 이미지를 포함하거나 다른 형태로 수정하세요! 😊
