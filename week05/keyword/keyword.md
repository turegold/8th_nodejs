# 🐜5주차 키워드

## 🐳환경변수
API 키나 계정의 ID, 비밀번호같은 기밀 정보를 있는 그대로 코드에 작성하거나, 기밀 정보가 담긴 코드를 Github와 같은 오픈소스에 공개하는 것은 보안적으로 위험하다.

dotenv는 . env라는 외부 파일에 중요한 정보를 환경변수로 저장하여 정보를 관리할 수 있게 해준다. 그래서 dotenv를 사용하면 전역적으로 필요한 정보나 기밀 정보와 같이 예민한 정보를 일반 소스 코드 내부가 아닌 .env라는 외부 파일에 작성할 수 있게 된다.

## 🍊CORS
Cross-Origin Resource Sharing의 줄임말로, 다른 출처간의 지원 공유를 허용할지 말지를 정하는 웹 보안 정책이다.

브라우저가 다른 출처의 API 요청을 기본적으로 막기 때문에 백엔드에서 cors 설정을 통해 특정 출처를 허용해야한다.

## ⏰DB Connection, DB Connection Pool
기존의 Connection 방식은 DB에 쿼리문을 보낼 때마다 Connection을 하고 결과를 받아왔지만, 이러한 방식은 비효율적이기 때문에 Connection Pool방식이 등장했다.

Connection Pool은 하나의 Pool을 생성한 뒤 지정한 수 만큼 Connection을 미리 할당한다.

그리고 Client에서 DB에 데이터를 가져오기위한 Connection을 Pool에서 가져와 사용한 뒤 다시 Pool에 Connection을 반환한다.

이렇게 Connection Pool 방식을 사용한다면 갑자기 동시접속자 수가 많아져도 에러를 발생시키지 않고, Pool에 남아있는 Connection이 없다면 대기상태가 되고 다른 클라이언트에서 Connection이 반환되면 대기상태가 풀리게된다.

## 🍔비동기 (async, await)
async, await은 자바스크립트에서 비동기 코드를 쉽게 작성하기 위한 문법.

동기로 작동하면 어떠한 작업을 할 때 응답이 올 때까지 기다려야 하니까, 다른 코드들이 멈춰버림.

하지만 비동기로 작동하면 기다리지 않고 다음 코드를 진행함.

과거에는 callback을 통해 Promise(내용이 실행은 되었지만 결과를 아직 반환하지 않은 객체)를 반환하였지만, 가독성이 떨어지기 때문에 현대에는 async/await을 사용한다.

await은 비동기 작업이 끝날 때까지 기다리게 하고, async는 그런 await을 사용하게 해준다.

## 🧑‍💻try/catch/finally
try 부분에는 문제가 생길 가능성이 있는 코드를 작성하고, catch 부분에서 에러가 발생했을 때 대응하는 코드를 작성한다. 마지막으로 finally 부분에는 성공이든 실패든 무조건 실행되는 부분이다.
