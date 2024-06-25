# 😀이건표 1차 프로젝트

### 🛒쇼핑몰 & 관리자 모드 기반 ChatBot 구현

# 🌟 **● 프로젝트 명** : E 1 I 4 🌟

#### **● 프로젝트 설명** : 원데이 클래스 강의 쇼핑몰 사이트
<img src="src/main/resources/static/images/메인.jpg" alt="프로젝트 메인 이미지"/>


## 개요 ✨
이 프로젝트는 평범한 물품 판매 사이트와 달리 강의 중심의 쇼핑몰 사이트를 구축하는 것을 목표로 하였습니다. 사용자 경험을 중시하며, 사용자의 지속적인 참여와 관리가 가능하도록 설계되었습니다.

## 목차 📚
- [프로젝트 배경](#프로젝트-배경-)
- [프로젝트 일정](#프로젝트-일정-)
- [팀원구성 및 역할](#팀원구성-및-역할-)
- [기술 스택](#기술-스택-)
- [주요 기능](#주요-기능-)
- [기능시연 영상](#기능시연-영상-)
- [향후 개선 사항](#향후-개선-사항-)


## 프로젝트 배경 📜
> 사용자에게 참신하고 편리한 서비스를 제공하기 위해 사용자 경험을 중심으로 한 웹사이트 디자인,
>
> 사용자와 관리자 간의 원활한 커뮤니케이션을 가능하게 하는 챗봇 시스템 등
>
> 더 투명하고 신뢰할 수 있는 정보를 제공하여 적극적인 참여를 유도하였다.

## 프로젝트 일정 🗓️
<img src="src/main/resources/static/images/일정.png" alt="프로젝트일정"/> 


## 팀원구성 및 역할 👥
- **(팀장) 박ㅇㅇ**: DB설계, 회원 CRUD, OAuth2, Security, CI/CD
- **(팀원) 심ㅇㅇ**: 게시판 CRUD (커뮤니티, 공지사항, 수강후기), NAVER API
- **(팀원) 손ㅇㅇ**: 관리자 페이지, Chatbot, 강사소개 페이지, 메뉴바, INDEX 애니메이션 기능
- **(팀원) 이건표**: 상품 CRUD, 장바구니 담당
- **(팀원) 조ㅇㅇ**: INDEX 페이지, 1:1 문의내역, NAVER API

## 기술 스택 🛠
<p align="center">
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white">
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">
<img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white">
<img src="https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
<img src="https://img.shields.io/badge/Amazon_AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white">
<img src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=Oracle&logoColor=white">
<img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=Spring-Security&logoColor=white">
<img src="https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white">
<img src="https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white">
<img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white">
<img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=for-the-badge&logo=Visual Studio Code&logoColor=white"/>
</p>
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

## 주요 기능 🚀
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

## 기능시연 영상 🎬

### 상점게시판 작성시연 영상
![1차create](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/3b2b3ba8-6853-402f-80b9-0acfa910ce60)

### 댓글작성 및 삭제
![1차댓글1](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/a368d7f1-5af9-476d-856f-a0182b233dce)

### 게시판 수정 삭제
![1차수정삭제](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/74b4892e-5b59-467d-8381-1b8d7d1326cc)

### 페이징 서치
![페이징서치](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/149e728e-f104-48cd-a9c5-238cad235db4)


### 좋아요 기능
![like](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/de5ef513-b8a0-427a-8569-06ce99fc6957)

### 장바구니
![장바구니](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/0fea4947-7feb-47cd-bffe-60bbb05d3bc9)

### 메인페이지 Top Like 순
![좋아요](https://github.com/leegeonpyo/Project_teamE1I4/assets/154856555/b65d4afd-632a-456f-8a24-b758c970f77d)

## 향후 개선 사항 🔧

프로젝트를 처음 시작할 때는 시간이 충분할 것이라 생각했지만, 예상보다 많은 기능을 구현하고 싶어하다 보니 시간 부족으로 인해 일부 기능을 완성하지 못하고, 디자인적으로도 만족스럽지 않은 부분들이 남아 아쉬움이 있습니다. 앞으로의 개선 사항은 다음과 같습니다:

1. **기능 완성도 향상**
    - 팀원들이 욕심 내어 계획했던 다양한 기능들을 완성하여, 사용자들에게 더욱 완벽한 서비스를 제공하고자 합니다.

2. **UI/UX 개선**
    - 시간에 쫓겨 포기했던 디자인 부분을 개선하여, 사용자들이 더 편리하고 직관적으로 이용할 수 있는 쇼핑몰 게시판을 구현하겠습니다.

3. **효율적인 시간 관리**
    - 프로젝트 일정 관리와 우선순위 설정을 통해, 제한된 시간 내에 최대한의 성과를 낼 수 있도록 하겠습니다.

4. **팀원들의 의견 반영**
    - 팀원들이 제안한 기능과 아이디어들을 최대한 반영하여, 팀원 모두가 만족할 수 있는 결과물을 만들어 나가겠습니다.

앞으로 프로젝트를 진행할 때는 이러한 개선 사항들을 바탕으로, 더 나은 결과물을 만들기 위해 노력하겠습니다.


**[⬆ 위로 가기](#이건표-1차-프로젝트)**