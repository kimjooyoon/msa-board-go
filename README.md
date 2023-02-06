# msa-board-go

### 소개

게시판 도메인에 대한 서비스 api 입니다.

아래 기능을 구성합니다.

- 게시판-카테고리: 읽기, 검색, 추가, 수정, 삭제
- 게시판-글: 읽기, 추가, 수정, 삭제

아래 권한 정책을 구성합니다.

- every: 게시판-글) 읽기, 검색 / 게시판-카테고리) 읽기
- owner: 게시판-글) 추가, 수정, 삭제
- admin: 게시판-카테고리) 추가, 수정, 삭제

### Docs

./msa-board-go.yaml

### Makefile

```makefile
build: # docker build msa-board-go:0.0.1
docker: # docker-compose up -d
push: # docker push github-package
```

### link

openApi spec 3.1: https://swagger.io/specification/

