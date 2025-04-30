# 🧑‍💻5주차 미션

### 1️⃣ **Controller 계층** (`handlerAddStore, handlerGetStore, handlerAddReview, handlerAddMission, handlerAdduserMission`)

- 📥 클라이언트의 요청을 받는 진입점 (HTTP 요청 수신)
- 요청 body를 `service`에 전달
- `service`의 결과를 받아서 응답(JSON)으로 반환

### 2️⃣ **Service 계층** (`addStore, addReview, addMission, addUserMission`)

- 💼 **비즈니스 로직**을 수행하는 계층
- 중복 가게 여부 확인, 실패 처리, 추가 후 정보 반환 등 로직 제어
- `repository` 함수를 호출해 DB와 실제로 연결

### 3️⃣ **Repository 계층** (`insertStoretoDB, getStorefromDB, insertReviewtoDB, getReviewfromDB, insertMissiontoDB, getMissionfromDB, insertUserMissiontoDB, getuserMissionfromDB`)

- 🛢️ **DB와 직접 통신하는 계층**
- SQL 쿼리 실행, 결과 반환
- 데이터베이스에 CRUD 역할만 충실히 수행

## 특정 지역에 가게 추가하기 API
![Image](https://github.com/user-attachments/assets/4b054522-fb9f-488f-a158-a15d23252840)

## 가게에 리뷰 추가하기 API
![Image](https://github.com/user-attachments/assets/affe1b69-ed3c-4ed1-bc23-6682ec372266)

## 가게에 미션을 추가하는 API
![Image](https://github.com/user-attachments/assets/2e386b11-e110-46d9-8b23-69cab6d3abf7)

## 가게에 미션을 도전중인 미션에 추가(미션 도전하기) API
![Image](https://github.com/user-attachments/assets/b84493e8-383a-44ab-be50-2d5b76bc39af)
![Image](https://github.com/user-attachments/assets/f8066998-ee1e-42cd-97f7-ce0a7bf8c540)
