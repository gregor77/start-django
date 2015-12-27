# django start project
about poll application

## runserver 실행방법
테스트용 웹서버인 runserver를 아래와 같이 실행 가능


```
$python manange.py runserver 0.0.0.0:8080
: 현재 실행중인 ip로 외부에서 접속 가능
```

```
$python manage.py runserver 0.0.0.0:8080 &
: '&'를 끝에 추가하면 백그라운드 실행
```

## admin
http://ip:port/admin을 입력하면 admin사이트로 이동가능하다.
로그인을 하려면 super user가 필요

#### 사용자, 사용자 그룹 테이블 생성
테이블을 만들지 않아도, 사용자 및 사용자 그룹 테이블을 만들기 위해 프로젝트 개발 처음에 실행 필요하다
```
$python manage.py migrate
```

#### super user 생성
```
$python manage.py createsuperuser
```
