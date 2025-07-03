# 연구실 홈페이지
## 로컬에서 빌드
이 홈페이지는 Jekyll 로 작성되어 있다. Jekyll 설치방법은 [여기를 참고](https://jekyllrb-ko.github.io/docs/).
```
bundle exec jekyll serve
```
위 커맨드로 빌드하고 `http://localhost:4000` 으로 접속하면 된다.
로컬에서 잘 동작하는지 확인하고 푸쉬나 PR 하도록 하자.

### (참고) Docker 이용방법
```sh
docker run --rm -it -p 4000:4000 \
    -e TZ=Asia/Seoul \
    -e PAGES_REPO_NWO="prosys/prosys.github.io" \
    -v "$PWD:/srv/jekyll" \
    jekyll/jekyll sh -c "chown -R jekyll /srv/jekyll && bundle install && bundle exec jekyll serve --host 0.0.0.0"
```

## Blog 쓰기
- `_data/authors.yml`에 본인의 정보를 기록
- `_post` 에 형식에 맞추어 글 작성
- `assets/yyyy-mm-dd/` 안에 필요한 그림 파일 등 저장
  - 이미지 확장자 대소문자를 통일해야 이미지 링크가 깨지지 않는다. 예를 들어 블로그 본문에 대문자 확장자를 사용해서 `![](/assets/path/to/picture.JPG)` 이름으로 이미지를 삽입한 경우 파일 확장자를 대문자 `picture.JPG` 로 저장해야한다.

## 블로그에 구글 포토 사진 첨부하기
대용량 사진을 이 저장소에 다 담기엔 불편하므로 구글 포토에 사진을 올리고 이를 링크하는 형식으로 블로그를 작성한다.

1. 연구실 구글 앨범 계정에 사진 올리기 (추후 졸업후에도 링크가 계속 유지되게)
  - 함께 만든 출장/행사 앨범이 있다면 거기에 넣기
  - 없다면 본인의 글에 쓸 앨범 만들기
3. 첨부할 사진이 있는 앨범이 공유가능한지 확인 (기본 설정이라면 공유가 가능)  
4. 구글 포토에서 첨부할 사진을 클릭하고 사진을 우클릭, **새 탭에서 이미지 열기**를 클릭
5. `lh3` 로 시작하는 링크에서 사진이 열리는 것을 확인. 해당 링크를 사용하면 사진 첨부 가능 (아래 예시 참고) 

    **예시** 
    ```
    | ![](https://lh3.googleusercontent.com/pw/AP1GczNQMNmcs9mxlzBqyVmLkAwmGSG8JREXqjDUOi5DgoEtf8h0xG7svFK92dwBsxbJ7YUN6WE0i768wXJzgKAZtR8OFpnipjEluLOrKppsCEXKNMOg0vruRNygdkTxAlCzhIgCs21j2tG9Kw-Lv8lnvrc_=w180-h180-s-no-gm?authuser=0) |
    |:--:|
    | <b> 연구실 로고 </b>|
    ```
    | ![](https://lh3.googleusercontent.com/pw/AP1GczNQMNmcs9mxlzBqyVmLkAwmGSG8JREXqjDUOi5DgoEtf8h0xG7svFK92dwBsxbJ7YUN6WE0i768wXJzgKAZtR8OFpnipjEluLOrKppsCEXKNMOg0vruRNygdkTxAlCzhIgCs21j2tG9Kw-Lv8lnvrc_=w180-h180-s-no-gm?authuser=0) |
    |:--:|
    | <b> 연구실 로고 </b>|


## Reference
[Template](https://github.com/mmistakes/mm-github-pages-starter)
