# Redmine Docker Composer Example

## Quick Start

**선행 조건** : 도커 및 도커 컴포즈 설치

### 인스턴스 시작하기

``` sh
# 환경 변수 설정 파일 복사
cp .env.example .env
# docker-compose 시작
docker-compose up
```

**선택 사항**

다음은 기본 제공 값 시드하는 방법입니다. 기본적인 이슈 유형과 역할 등을 시딩하빈다.

``` sh
# redmine docker instance에 접속
# docker instance 이름은 보통 redmine_redmine_1 이지만
#적절하게 변경 할 필요가 있으면 알 맞게 대응 하세요.
docker exec -it redmine_redmine_1 /bin/bash
rake redmine:load_default_data
```

빠저나오기를 하려면 `ctrl`+`d` 단축키 사용 
혹은 `exit` 명령어 사용

### 접속 하기

http://localhost:8080

**초기 admin 계정**
id/password : admin/admin
