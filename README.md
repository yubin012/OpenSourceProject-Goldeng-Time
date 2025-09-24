# 골댕타임 (Goldaeng Time)
실종 반려동물 발견 및 매칭 플랫폼
**팀원:** 32212398 심예린, 32215080 박유빈

---

## 프로젝트 개요 
<img width="915" height="496" alt="image" src="https://github.com/user-attachments/assets/087a17f0-721e-48b2-8d92-693c0f1d4434" />
<img width="895" height="508" alt="image" src="https://github.com/user-attachments/assets/1e315d03-0a6f-4057-9434-b2d848a68c40" />
<img width="871" height="480" alt="image" src="https://github.com/user-attachments/assets/0468e6d6-20aa-4b5e-8ff0-090857af8b40" />
반려동물 실종 시 전단지와 SNS에 의존하는 기존 방식의 한계를 극복하고, AI와 GPS 기반 위치 정보를 활용하여 실종 반려동물을 빠르고 효율적으로 찾을 수 있는 플랫폼을 개발하였습니다.  
서비스 이름 ‘골댕타임’은 골든타임과 반려동물 멍멍이(댕댕이)를 결합한 명칭입니다.
---

## 주요 기능
### 1. 반려자(주인) 기능
- 반려동물 등록 (사진, 특징, 품종 등)
- 실종 게시글 작성 및 상태 관리
- 실시간 푸시 알림

### 2. 목격자 기능
- 발견 게시글 작성 (사진, 위치, 특징)

### 3. 공통 기능
- AI 기반 실시간 유사도 매칭
- 지도 기반 시각화 및 실시간 위치 업데이트
- 댓글/답글, 게시글 스크랩, 마이페이지 관리

---

## 기술 스택
<img width="893" height="515" alt="image" src="https://github.com/user-attachments/assets/dbdcc48e-164a-478d-ab29-5bce7c7a6a99" />

- **Backend:** Spring Boot, RESTful API  
- **DB:** MySQL, AWS RDS  
- **AI:** Google Cloud Vision API (이미지 유사도 분석)  
- **알림:** Firebase Cloud Messaging (FCM)  
- **배포/환경:** Docker, GitHub Actions  

---

## ERD
<img width="712" height="731" alt="image" src="https://github.com/user-attachments/assets/4f58cef2-f938-42f3-a8b8-a067754f3b6b" />
 
사용자, 반려동물, 실종/발견 게시글, 댓글, 스크랩, 매칭 정보를 구조화하여 관리

---

## 상세 구현
1. Spring Security + JWT 기반 인증/인가
2. 반려동물 등록 및 게시글 관리
3. Google Cloud Vision API로 이미지 유사도 계산
4. FCM을 통한 매칭 푸시 알림 전송
5. 댓글 및 대댓글 구조 구현
6. Docker 컨테이너 기반 개발 환경 구축
7. GitHub Actions를 통한 CI/CD 자동화

---

## 구현 화면
### 메인 화면 , 홈 & 지도 화면
<img width="902" height="507" alt="image" src="https://github.com/user-attachments/assets/92d6846b-d16b-4d9b-9402-2f62cfc34fdf" />


### 반려동물 등록 화면 & 실종/발견 게시글 작성
<img width="898" height="411" alt="image" src="https://github.com/user-attachments/assets/5890cbc4-e184-4747-893d-5a7fda1fa063" />

### 유사도 매칭 & 푸시 알림
<img width="851" height="415" alt="image" src="https://github.com/user-attachments/assets/3253f890-bcbb-4b9b-89fd-a636b986a8ab" />


### 마이페이지
<img width="717" height="412" alt="image" src="https://github.com/user-attachments/assets/eb8242d6-487a-4bcb-a528-b3efef8ad423" />

---

## 발표 자료
[전체 PPT 다운로드]
[최종발표자료_수정 (1).pdf](https://github.com/user-attachments/files/22508355/_.1.pdf)

---

## 테스트 결과
- 회원가입, 로그인, JWT 인증: 정상 작동
- 게시글 CRUD 및 댓글/답글 처리: 정상 작동
- 게시글 스크랩 및 매칭 푸시 알림: 정상 작동 (유사도 85% 이상)
- Swagger/Postman API 테스트 완료
 <img width="680" height="617" alt="image" src="https://github.com/user-attachments/assets/2a666a0a-0045-4c0e-b309-e8c3eaacbc86" />
 <img width="687" height="827" alt="image" src="https://github.com/user-attachments/assets/0cce9f0e-4c7c-43e9-8c6b-02a3c5f543f6" />


- Google Cloud Vision API 부하 테스트 및 MySQL 대용량 조회 테스트 완료

---

## 참고 문헌
1. [Google Cloud Vision API 공식 문서](https://cloud.google.com/vision/docs)  
2. [Firebase Cloud Messaging 공식 문서](https://firebase.google.com/docs/cloud-messaging)  
3. [Spring Boot 공식 문서](https://spring.io/projects/spring-boot)  
4. [Swagger OpenAPI 공식 문서](https://swagger.io/specification/)
