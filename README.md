# SPRING ADVANCED

## Lv 0. 에러 분석

### 발생한 에러 목록
1. `Could not resolve placeholder 'jwt.secret.key'`
    - 원인: `resources` 폴더와 `application.properties` 파일 누락
    - 해결: 파일 생성 후 jwt 키 추가

2. `Failed to configure a DataSource`
    - 원인: DB 접속 정보 누락
    - 해결: MySQL 설정 추가

3. 환경변수 오타 `JWT_SECRET_KET` → `JWT_SECRET_KEY`
    - 원인: IntelliJ 환경변수 이름 오타
    - 해결: 환경변수 이름 수정