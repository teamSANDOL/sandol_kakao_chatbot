# 📌 산돌이 Repository Template  

## 📂 개요 
산돌이 카카오톡 챗봇 서버 Repository입니다.

---

## 📌 프로젝트 구조  
- FastAPI, SQLite, SQAlchemy, 
- [카카오톡 Open Builder](https://chatbot.kakao.com/bot/67217ff5fb73245c1c65e60f)

---

## 📌 문서  
이 서버의 문서는, KakaoOpenbuild와 서버의 Skill 및 파라미터 정보를 제공합니다.
- [API 문서 (Notion)](링크)
- [API 문서 (Swagger)](링크)
- 참고 문서
  - [파이썬 kakao-chatbot 패키지 문서](kakao-chatbot.readthedocs.io)

---

## 📌 환경 설정  
- **모든 서비스는 Docker 기반으로 실행되므로, 로컬 환경에 별도로 의존하지 않음**  
- **환경 변수 파일 (`.env`) 필요 시, 샘플 파일 (`.env.example`) 제공**  
- **Docker Compose를 통해 서비스 간 네트워크 및 볼륨을 설정**  
- **프론트엔드 서비스(챗봇 서버, 웹 서비스)와 백엔드 서비스(API 서버)의 차이점을 반영하여 개별 실행 가능**  

### 📌 실행 방법  
#### 1. 기본 실행 (모든 서비스 실행)  
```bash
docker compose up -d
```
#### 2. 특정 서비스만 실행 (예: 챗봇 서버)  
```bash
docker compose up -d <서비스명>
```
#### 3. 서비스 중지  
```bash
docker compose down
```
#### 4. 환경 변수 변경 후 재시작  
```bash
docker compose up -d --build
```

---

## 📌 배포 가이드  
- **(CI/CD 적용 여부 및 배포 자동화 여부를 설명하세요.)**  
  - 예시: `GitHub Actions 사용 여부`, `GCP Cloud Run 자동 배포`, `AWS Lambda 연동 여부` 등  
- **(배포 시 관리해야 할 환경 변수 및 보안 설정을 명시하세요.)**  
  - 예시: `.env 파일의 API Key`, `Webhook URL`, `DB 접속 정보` 등
- **(배포시 주의해야할 사항을 설명하세요.)**
  - 예시: `별도 domain 연결 필요`, `독립 Database 설정 필요` 등
---

## 📌 문의  
- [디스코드 카카오 챗봇 채널](https://discord.com/channels/1339452791071969331/1339456512363597875)

---
🚀 **산돌이 프로젝트와 함께 효율적인 개발 환경을 만들어갑시다!**  
