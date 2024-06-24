# 🌟 E1I4TeamProject 🌟

<p align="center">
  <img src="src/main/resources/static/images/메인.jpg" alt="프로젝트 메인 이미지"/>
</p>

## 개요 ✨
이 프로젝트는 평범한 물품 판매 사이트와 달리 강의 중심의 쇼핑몰 사이트를 구축하는 것을 목표로 하였습니다. 사용자 경험을 중시하며, 사용자의 지속적인 참여와 관리가 가능하도록 설계되었습니다.

## 목차 📚
- [프로젝트 배경](#프로젝트-배경)
- [팀원구성 및 역할](#팀원구성-및-역할)
- [기술 스택](#기술-스택-🛠)
- [주요 기능](#주요-기능)
- [기능시연 영상](#기능시연-영상)
- [향후 개선 사항](#향후-개선-사항)
- [연락처](#연락처)

## 프로젝트 배경 📜
이 프로젝트는 평범한 물품 판매 사이트와 달리 강의 중심의 쇼핑몰 사이트를 구축하는 것을 목표로 하였습니다. 사용자 경험을 중시하며, 사용자의 지속적인 참여와 관리가 가능하도록 설계되었습니다.

## 팀원구성 및 역할
- **(팀장) 박ㅇㅇ**: DB설계, 회원 CRUD, OAuth2, Security, CI/CD
- **(팀원) 심ㅇㅇ**: 게시판 CRUD (커뮤니티, 공지사항, 수강후기), NAVER API
- **(팀원) 손ㅇㅇ**: 관리자 페이지, Chatbot, 강사소개 페이지, 메뉴바, INDEX 애니메이션 기능
- **(팀원) 이건표**: 상품 CRUD, 장바구니 담당
- **(팀원) 조ㅇㅇ**: INDEX 페이지, 1:1 문의내역, NAVER API

## 기술 스택 🛠
- **프로젝트명**: E1i4TeamProject
- **프로그래밍 언어**: JAVA
- **프레임워크**: Springboot 2.7.11
- **라이브러리**: Spring WEB(MVC), Thymeleaf, Spring Data JPA, Lombok, SpringSecurity5, websocket, validation, OAuth2, security
- **데이터베이스**: MySql8
- **ORM**: Spring Data JPA (JAVA(SQL))
- **개발툴**: IntelliJ
- **템플릿 엔진**: Thymeleaf (HTML + Data)
- **빌드**: Gradle
- **설정**: application.yml, application-oauth2.yml

## 주요 기능
### SHOP(CRUD)
| NO | 기능         | 설명                                                                 |
|----|--------------|----------------------------------------------------------------------|
| 1  | 게시판작성   | 클래스를 미술, 체육, 음악, 요리 카테고리로 분류<br>선생님명은 회원닉네임으로 자동표기<br>파일선택으로 게시글 사진추가 |
| 2  | 게시판조회   | 게시글 상세 조회 가능<br>게시글을 좋아요를 눌러 찜 가능<br>게시글 조회수 추가<br>게시글 댓글 기능 추가 작성 및 삭제 구현<br>수량 체크 후 개수만큼 장바구니로 이동 구현 |
| 3  | 게시판수정   | 제목, 내용, 카테고리, 금액, 인원, 사진 수정 가능                     |
| 4  | 게시판삭제   | 본인이 작성한 게시글만 삭제 가능                                     |
| 5  | 게시판좋아요 | 토글 방식으로 게시글당 한 번만 좋아요 가능<br>다시 누를 경우 취소 구현<br>좋아요를 통해 메인페이지에 이달의 랭킹 순위에 게시글 표시 |
| 6  | 게시판조회수 | 조회수 기능 추가, 게시글 한 번 들어갈 때마다 +1                     |

### CART
| NO | 기능           | 설명                                                   |
|----|----------------|--------------------------------------------------------|
| 1  | 장바구니 생성  | 게시판에서 장바구니 담기 누르면 카트 자동 생성        |
| 2  | 장바구니 삭제  | 장바구니에서 개별 목록 삭제와 전체 삭제 기능 구현     |
| 3  | 장바구니 조회  | 장바구니로 이동 시 자기가 담은 장바구니 리스트 확인 가능 |

## 기능시연 영상

### 상점게시판 작성시연 영상
<img src="https://private-user-images.githubusercontent.com/154856555/342218564-971acb3d-ae12-4bba-bad9-f243c4ca71e1.gif">

### 댓글작성 및 삭제
<img src="https://private-user-images.githubusercontent.com/154856555/342241984-832f4714-1b5e-4ebc-bf41-16187307bd51.gif">

### 게시판 수정 삭제
<img src="https://private-user-images.githubusercontent.com/154856555/342243111-7f489686-a39c-478b-a8c2-25d87009fa7a.gif">

### 페이징 서치
<img src="https://private-user-images.githubusercontent.com/154856555/342255255-bb3d9265-5bc7-43d5-af65-5f37414ddca6.gif">

### 좋아요 기능
<img src="https://private-user-images.githubusercontent.com/154856555/342256046-813620f4-e56f-4647-ab07-f39975ef45eb.gif">

### 장바구니
<img src="https://private-user-images.githubusercontent.com/154856555/342258814-1e571c8c-1b55-42e2-aac5-4d0a388f18e4.gif">

### 메인페이지 Top Like 순
<img src="https://private-user-images.githubusercontent.com/154856555/342259533-e4e7cbee-fec1-4894-bd66-468beee17236.gif">

## 향후 개선 사항
프로젝트 처음 시작할 때는 시간이 많은 줄 알았습니다. 첫 프로젝트이기도 하고, 우리 팀원들이 욕심이 많아서 하고 싶은 것들이 많다 보니 생각보다 구현하지 못한 것이 많고, 더 예쁘게 할 수 있었는데 시간에 쫓겨서 포기한 것이 많아서 아쉽습니다. 더 사용자들에게 편리한 쇼핑몰 게시판으로 구현하고 싶습니다.

## 연락처
추가적인 문의나 정보가 필요하시면 아래 연락처로 연락해 주세요.

- 이메일: example@example.com
- 전화번호: 010-1234-5678
