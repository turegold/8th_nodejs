# 🐳8주차 키워드

## 🐜Swagger
Swagger는 개발한 Rest API를 편리하게 문서화해주고, 이를 통해서 관리 및 API를 편리하게 테스트할 수 있는 도구 및 프레임워크이다. Swagger는 API 문서 자동화, API 테스트 인터페이스 제공, 개발자간의 협업 효율 증가, 서버/클라이언트 코드 자동 생성 가능이라는 장점을 갖고있다.

## 🐶OpenAPI
OpenAPI는 OpenAPI Specification(OAS)라고도 부르는데, 이는 RESTful API를 정의된 규칙에 맞게 API spec을 json이나 yaml 형식으로 표현하는 방식을 의미한다. 이 문서를 통해 API 문서 자동 생성, 코드 생성(서버/클라이언트), 테스트 UI 생성 (Swagger UI) 등이 가능하다.

## 🧑‍💻OpenAPI Component
OpenAPI에서 components는 공통으로 재사용할 수 있는 데이터 구조(스키마, 응답, 파라미터 등)를 정의하는 영역이다. 모든 API 응답에서 resultType, error와 같이 중복되는 구조가 존재한다면, components에 이것들을 정의해두고 $ref를 통해 불러와서 사용할 수 있다. OpenAPI 3.0 기준으로 components안에는 schemas(객체 구조), parameters(쿼리, 경로, 헤더 등), responses(응답 형식), requestBodies(요청 바디 형식), securitySchemes(인증 방식 정의)를 정의할 수 있다.
.
