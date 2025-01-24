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

## 7. Client 화면 구성

### **1. Main Page**
- 메인 페이지는 로그인된 사용자가 프로젝트와 유저 관리를 선택할 수 있는 페이지입니다.
- 주요 기능:
  - 프로젝트 관리 페이지로 이동
  - 사용자 관리 페이지로 이동

![Main Page](images/main_page.png)

---

### **2. User Management Page**
- 사용자 관리 페이지에서는 회사에 소속된 사용자들을 관리할 수 있습니다.
- 주요 기능:
  - 사용자 추가 및 삭제
  - 특정 사용자에 대한 세부 정보 조회

![User Management Page](images/user_management_page.png)

---

### **3. Project Management Page**
- 프로젝트 관리 페이지는 회사 내 모든 프로젝트와 관련된 정보를 표시합니다.
- 주요 기능:
  - 프로젝트 생성 및 삭제
  - 프로젝트에 대한 세부 정보 조회
  - 프로젝트 참여자 관리

![Project Management Page](images/project_management_page.png)
## 8. Docker Deployment

### Docker Deployment Diagram
![Docker Deployment](images/docker_deployment.png)

### Docker Sequence Diagram
![Docker Sequence](images/docker_sequence.png)

### Docker Hub Push
![Docker Hub Push](images/docker_hub_push2.png)

---

### Docker 실행 및 작동
1. **Docker 실행 및 작동 1**
   ![Docker 실행 1](images/docker_run_2.png)

2. **Docker 실행 및 작동 2**
   ![Docker 실행 2](images/docker_run_3.png)

3. **Docker 실행 및 작동 3**
   ![Docker 실행 3](images/docker_run_4.png)


---

## 8. 추가 참고사항
- 각 이미지를 `images/` 디렉토리에 저장하여 Markdown 파일과 동일 디렉토리 구조에서 참조하세요.
- 실제 이미지 파일을 해당 경로에 복사하거나, 이미지 링크를 업데이트하세요.
