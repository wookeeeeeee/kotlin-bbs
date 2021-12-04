# Kotlin BBS

## 주요 사용 기술 및 방법

* spring-boot with kotlin
* jpa
* h2 database
* tdd

## 구현목록

* [x] 게시글 등록
    * [x] 작성자 제목 내용으로 게시글을 등록한다
    * [x] 작성자 제목 내용이 없으면 예외가 발생한다
* [x] 게시글 목록 조회
* [x] 게시글 조회
    * [x] 게시글이 없으면 예외가 발생한다
* [x] 게시글 수정
    * [x] 제목 내용을 수정한다
* [ ] 게시글 삭제
    * [ ] 게시글 아이디로 게시글을 삭제한다
    * [ ] 삭제할 게시글이 없으면 예외가 발생한다
* [ ] 댓글 등록
    * [ ] 게시글에 댓글을 등록한다
    * [ ] 댓글을 등록할 게시글이 없으면 예외가 발생한다
* [ ] 댓글 목록 조회
* [ ] 댓글 수정
    * [ ] 댓글의 내용을 수정한다
    * [ ] 수정할 댓글이 없으면 예외가 발생한다
* [ ] 댓글 삭제
    * [ ] 댓글의 아이디로 댓글을 삭제한다
    * [ ] 삭제할 댓글이 없으면 예외가 발생한다
* [ ] 게시글 좋아요
    * [ ] 게시글 좋아요를 한다
    * [ ] 좋아요할 게시글이 없으면 예외가 발생한다
    * [ ] 이미 게시한글에 좋아요를 하면 예외가 발생한다
* [ ] 게시글 좋아요 취소
    * [ ] 게시글 좋아요를 취소한다
    * [ ] 좋아요를 취소할 게시글이 없으면 예외가 발생한다

> Board -> 게시글 Comment -> 댓글 Like -> 좋아요
>
> Like는 게시글에 대해서 좋아요를 한것에 대한 정보이고 제가 좋아요 누르면 저의 이름으로 Entity가 저장이 되는거죠
>
> Board에서는 Comment의 정보를 모르고 있게 (OneToMany 사용 X)
>
> Board에서는 Like의 정보를 모르고 있게 (OneToMany 사용 X)