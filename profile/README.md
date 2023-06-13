# 🤓 충남대 역량 폼 미쳤다
<div align="center">
  <img src="https://github.com/perfume-site-project/perfume-website/assets/33623123/737c767e-9125-42ed-9025-55b3287a2f42">
<!--   ![logo_+cnu](https://github.com/perfume-site-project/perfume-website/assets/33623123/737c767e-9125-42ed-9025-55b3287a2f42) -->
</div>


# CNU Archive Web Page v1.0
> **충남대학교 공공데이터 활용경진대회** <br/> **개발기간: 2023.04 ~ 2023.06**


## 배포 주소
> **개발 버전** : 예정<br>
> **프론트 서버** : 예정<br>
> **백엔드 서버** : 예정<br>


## 👨‍👨‍👧‍👧 팀 소개
|      강병현       |          박신욱         |       이은경        |        김대민        |                                                                                                               
| :------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   <img width="160px" src="https://avatars.githubusercontent.com/u/33623123?v=4" />    |                      <img width="160px" src="https://github.com/cnu-data-contest/.github/assets/33623123/d002486e-dd84-4fe1-8509-1260409f46b2" />    |                   <img width="160px" src="https://avatars.githubusercontent.com/u/81898507?v=4"/>   |                   <img width="160px" src="https://avatars.githubusercontent.com/u/56399681?v=4"/>   |
|   [@llbllhllk](https://github.com/llbllhllk)   |    [@hwibaluuu](https://github.com/hwibaluuu)  | [@pkyung](https://github.com/pkyung)  | [@daemin-kim](https://github.com/daemin-kim)  |
| 충남대학교 컴퓨터공학과 4학년 | 충남대학교 디자인창의학과 4학년 | 충남대학교 컴퓨터융합학부 3학년 | 충남대학교 컴퓨터융합학부 3학년 |
| FE (팀장) | UI/UX (팀원) | BE (팀원) | BE (팀원) |

## 서비스 소개
충남대학교의 모든 학과의 교내활동을 한 곳에 집약해놓은 플랫폼이다.
(더 자세히 쓸예정....)


## Stacks 🐈
<!-- 아래 참고해서 Stack추가해줘! -->
<!-- https://simpleicons.org/ -->
<!-- <img src="https://img.shields.io/badge/표시할이름-색상?style=for-the-badge&logo=기술스택아이콘&logoColor=white"> -->
### Environment
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-007ACC?style=for-the-badge&logo=Visual%20Studio%20Code&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=Git&logoColor=white)
![Github](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=white)             

### Config
![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)        

### Development
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=Javascript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
<img src="https://img.shields.io/badge/styled components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white">
<img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> 

### Communication
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=Notion&logoColor=white)
<img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=Discord&logoColor=white">

---
## 화면 구성 📺
| 로그인 페이지  |
| :-------------------------------------------: |
|  <img width="1000" src="https://github.com/llbllhllk/diary/assets/33623123/a85226ec-533d-4114-8317-662857386a73"/> |
|  관심학과 선택 페이지   |
|    <img width="1000" src="https://github.com/llbllhllk/diary/assets/33623123/a9fedd5c-c235-4222-bd2b-dea027e4d5dd"/>|
|  메인 페이지   |
| <img width="1000" src="https://github.com/llbllhllk/diary/assets/33623123/86b6bd67-fd1e-47b5-af79-afafd0ad637e"/>   |
---
## 주요 기능 📦

### ⭐️ 강좌 선택 및 강의 영상 시청 기능
- Scratch, Python 2개 강좌 및 각 강좌마다 10개 가량의 강의 영상 제공
- 추후 지속적으로 강좌 추가 및 업로드 예정

### ⭐️ 강의 관련 및 단체에 대한 자유로운 댓글 작성 가능
- Disqus를 이용하여 강의 관련 질문이나 단체에 대한 질문 작성 가능

### ⭐️ 이어 학습하기 기능
- Cookie 기능을 이용하여 이전에 학습했던 내용 이후부터 바로 학습 가능

---

## 아키텍쳐
### 디렉토리 구조
```bash
├── README.md
├── package-lock.json
├── package.json
├── strapi-backend : 
│   ├── README.md
│   ├── api : db model, api 관련 정보 폴더
│   │   ├── about
│   │   ├── course
│   │   └── lecture
│   ├── config : 서버, 데이터베이스 관련 정보 폴더
│   │   ├── database.js
│   │   ├── env : 배포 환경(NODE_ENV = production) 일 때 설정 정보 폴더
│   │   ├── functions : 프로젝트에서 실행되는 함수 관련 정보 폴더
│   │   └── server.js
│   ├── extensions
│   │   └── users-permissions : 권한 정보
│   ├── favicon.ico
│   ├── package-lock.json
│   ├── package.json
│   └── public
│       ├── robots.txt
│       └── uploads : 강의 별 사진
└── voluntain-app : 프론트엔드
    ├── README.md
    ├── components
    │   ├── CourseCard.js
    │   ├── Footer.js
    │   ├── LectureCards.js
    │   ├── MainBanner.js : 메인 페이지에 있는 남색 배너 컴포넌트, 커뮤니티 이름과 슬로건을 포함.
    │   ├── MainCard.js
    │   ├── MainCookieCard.js
    │   ├── NavigationBar.js : 네비게이션 바 컴포넌트, _app.js에서 공통으로 전체 페이지에 포함됨.
    │   ├── RecentLecture.js
    │   └── useWindowSize.js
    ├── config
    │   └── next.config.js
    ├── lib
    │   ├── context.js
    │   └── ga
    ├── next.config.js
    ├── package-lock.json
    ├── package.json
    ├── pages
    │   ├── _app.js
    │   ├── _document.js
    │   ├── about.js
    │   ├── course
    │   ├── index.js
    │   ├── lecture
    │   ├── newcourse
    │   ├── question.js
    │   └── setting.js
    ├── public
    │   ├── favicon.ico
    │   └── logo_about.png
    └── styles
        └── Home.module.css

```
### 아키텍처 상세
![소프트웨어아키텍처](https://user-images.githubusercontent.com/33623123/181793237-1ce39f8e-ce78-47f0-8f7d-1e93953c379c.jpg)

