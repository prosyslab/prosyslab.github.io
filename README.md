# 연구실 홈페이지
## 로컬에서 빌드
이 홈페이지는 Jekyll 로 작성되어 있다. Jekyll 설치방법은 [여기를 참고](https://jekyllrb-ko.github.io/docs/).
```
bundle exec jekyll serve
```
위 커맨드로 빌드하고 `http://localhost:4000` 으로 접속하면 된다.
로컬에서 잘 동작하는지 확인하고 푸쉬나 PR 하도록 하자.

## Blog 쓰기
- `_data/authors.yml`에 본인의 정보를 기록
- `_post` 에 형식에 맞추어 글 작성
- `assets/yyyy-mm-dd/` 안에 필요한 그림 파일 등 저장

위 커밋을 PR 로 보낸다

## Reference
[Template](https://github.com/mmistakes/mm-github-pages-starter)
