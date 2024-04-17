<div>
  <h1> 금융 데이터 기반 티켓 할인 예매 사이트 Ticketpong </h1>
<h3>프로젝트 소개</h3>
  <li> 티켓 예매 사이트 티켓퐁은 독점 방지를 위한 예매사이트 분산의 필요성과 소비자 편의성 제공을 목적으로 시작했습니다. </li>
  <li> 문화생활에 대한 접근성을 높일 수 있는 정보 집약적 서비스 구현을 목표로 하고 있습니다.</li>
  <li> 로그인을 하지 않더라도, 공연예정 일정이나 잔여 티켓 확인이 가능합니다.</li>
  <li> 회원가입시, 기기등록을 통해 티켓예매 및 예매기록을 통해 공연에 대한 리뷰 등록이 가능합니다.</li>
  <li> 티켓 예매시 기기 등록을 통해 예매숫자를 제한하고 있습니다.</li>
</div>

<hr>

### 팀원 구성
| 황인식 | 손지연 |  박우정   |  이예리  |  양재식   |  송운정   |
| :--------: | :--------: | :------: | :-----: | :-----: | :-----: |
|  조장 |   백엔드    | 백엔드 | 프론트 | 프론트 | 프론트 |

<hr>

<div>
  <h3>1. 개발 환경</h3>
  <div>
  <span>Front</span>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white">
<img src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=whit">
<img src="https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white">
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB">
<div>
<div >
  <span>Back-end</span>
<img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white">
<img src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white">
<img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white">
<img src="https://img.shields.io/badge/Express.js-404D59?style=for-the-badge">
</div>
<div>
  <span>협업 툴</span>
<img src="	https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white">
<img src="https://img.shields.io/badge/Zoom-2D8CFF?style=for-the-badge&logo=zoom&logoColor=white">
<img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white">
</div>

<hr>

<div>
  <h3>2.  채택한 개발 기술과 브랜치 전략</h3>
  <h4>React, styled-component</h4>
  <ul>
    <h4>React</h4>
    <li>컴포넌트화를 통해 추후 유지보수와 재사용성을 고려했습니다</li>
    <li>유저 배너, 상단과 하단 배너 등 중복되어 사용되는 부분이 많아 컴포넌트화를 통해 리소스 절약이 가능했습니다.</li>
  </ul>
  <ul>
    <h4>Styled-component</h4>
    <li>props를 이용한 조건부 스타일링을 활용하여 상황에 알맞은 스타일을 적용시킬 수 있었습니다.</li>
    <li>빌드될 때 고유한 클래스 이름이 부여되어 네이밍 컨벤션을 정하는 비용을 절약할 수 있었습니다.</li>
  </ul>
  <h4>eslint, prettier</h4>
  <li>정해진 규칙에 따라 자동적으로 코드 스타일을 정리해 코드의 일관성을 유지하고자 했습니다.</li>
  <li>코드 품질 관리는 eslint에, 코드 포맷팅은 prettier에 일임해 사용했습니다.</li>
  <h4>브랜치 전략</h4>
  <li>Git-flow 전략을 기반으로 main, develop 브랜치와 feature 보조 브랜치를 운용했습니다.</li>
  <li>main 브랜치는 배포 단계에서만 사용하는 브랜치입니다.</li>
  <li>develop 브랜치는 개발 단계에서 git-flow의 master 역할을 하는 브랜치입니다.</li>
  <li>Feat 브랜치는 기능 단위로 독립적인 개발 환경을 위하여 사용하고 merge 후 각 브랜치를 삭제해주었습니다.</li>
</div>

<hr>

### 3.  프로젝트 구조

#### Front

- README.md
- src
   - App.css
   - App.js
   - assets
      - footerImg
         - arrowIcon.png
      - headerImg
         - header_userIcon.png
         - logo.png
         - menuIcon.png
         - nav_commIcon.png
         - nav_showIcon.png
         - nav_userIcon.png
         - poster_sample.jpg
      - homeImg
         - free-icon-like-179655.png
         - mainImg_01.jpg
         - mainImg_02.jpg
         - searchIcon_p.png
         - searchIcon_w.png
      - searchResultImg
         - posterImg.jpg
         - search_topImg.jpg
      - ViewAllImg
         - Image20240328164620.jpg
   - components
      - base
         - ApiDataFetcher.js
         - axiosWithAuth.js
         - Footer.js
         - Header.js
         - KakaoMap.js
         - SearchBar.js
         - WriteReview.js
      - features
         - Community
            - CommunityBoard.js
            - CommunityRules.js
            - CommuReview.js
            - ReviewDetail.js
         - Header
            - NavMenu.js
            - UserMenu.js
         - HomePage
            - HPContent1.js
            - HPContent2.js
            - HPReviews.js
            - MainImg.js
         - ManagePage
            - AdminManage.js
            - EditManage.js
            - ManageAdd.js
            - MemberManage.js
            - PerformanceChg.js
            - PerformanceManage.js
            - PerformanceReg.js
            - ReviewDetail.js
            - ReviewManage.js
         - MyPage
            - BookingDetail.js
            - BookingDetailModal.js
            - EditMyReview.js
            - EditProfile.js
            - MyReview.js
            - PwCheck.js
            - SetDevice.js
         - Ticketing
            - css
               - TicketingCalendar.css
            - SeatSelectionModal.js
            - ShowSchedule.js
            - TicketingCalendar.js
            - TicketingHeader.js
            - TicketingPayment.js
            - TicketingReview.js
            - TicketingSelectSeat.js
            - TicketingShowInfo.js
   - index.js
   - pages
      - community
         - Community.js
      - findidpw
         - ConfirmId.js
         - FindId.js
         - FindPw.js
      - homepage
         - HomePage.js
      - managepage
         - ManageLoginPage.js
         - ManagePage.js
      - manageuser
         - LoginPage.js
         - SignupPage.js
      - mypage
         - MyPage.js
      - performance
         - Performance.js
      - searchresult
         - SearchResult.js
      - ticketing
         - Ticketing.js
   - styles
      - FooterStyled.js
      - HeaderStyled.js
      - PerformanceStyled.js
      - SearchAllStyled.js
      - SearchHomeStyled.js
      - TicketingStyled.js

<hr>

#### Back-end

- .env
- app.js
- config
   - mariadb.js
- controllers
   - apiController.js
   - findIdPasswordController.js
   - homepageController.js
   - infoController.js
   - loginController.js
   - macAddressController.js
   - performanceController.js
   - reservationController.js
   - reviewController.js
   - searchBarController.js
   - signupController.js
   - viewAllController.js
- model
   - dbconnect.js
   - dbPool.js
- package-lock.json
- package.json
- README.md
- routes
   - api.js
   - homepage
      - homepage.js
   - index.js
   - manage
      - manageAdd.js
      - manageLogin.js
      - manageLogout.js
      - manageMain.js
   - member
      - findIdPassword.js
      - login.js
      - logout.js
      - macAddress.js
      - main.js
      - signup.js
   - reservation
      - reservation.js
   - review.js
   - searchBar.js
   - viewall.js
- service
   - api
      - hallService.js
      - resService.js
      - showService.js
   - findIdPasswordService.js
   - homepageService.js
   - infoService.js
   - loginService.js
   - macAddressService.js
   - manageService.js
   - performanceService.js
   - reservationService.js
   - reviewService.js
   - searchBarService.js
   - signupService.js
   - viewAllService.js
- sessions

<hr>

### 4.  역할 분담

#### 황인식

<li>상세페이지(예매, 결제, 상세)</li>
<li>마이페이지(예매확인, 후기, 사용자 기기 등록/수정)</li>
<li>관리자페이지(후기), 총괄</li>

#### 손지연
<li>DB 설계 및 연결</li>
<li>로그인 및 회원가입 기능 구현</li>
<li>ID/PW 찾기 기능 구현</li>
<li>관리자 페이지(관리자 기능)</li>
<li>회원 정보 수정 페이지</li>

#### 양재식

<li>메인페이지(슬라이더배너/후기)</li>
<li>전체보기 페이지(공연 리스트)</li>
<li>커뮤니티(공지,후기,이용안내)</li>

#### 박우정

<li>DB설계</li>
<li>관리자 페이지(회원관리, 공연관리)</li>

#### 이예리 

<li>Figma, ppt 디자인</li>
<li>Header, Footer</li>
<li>ID/PW 찾기 화면 구현</li>
<li>메인페이지 상단배너</li>
<li>검색창 및 검색 기능</li>

#### 송운정

<li>디자인 설계</li>
<li>스타일 가이드 작성</li>

<hr>

### 5.  개발 기간 및 작업 관리

#### 전체 개발 기간
<li>2024.03.12 ~ 2024.04.17 </li>
<li>UI 구현: </li>
<li>기능 구현: </li>

#### 작업 관리

<li>Zoom을 이용해서 실시간 소통을 하면서 상황을 공유하며 진행했습니다.</li>
<li>Git-flow 전략을 기반으로 main, feature, develop 브랜치를 운용했습니다. </li>

<hr>

### 6. 기능 설명

#### [Header]
<li> useEffect와 axiosWithAuth를 이용, 사용자 인증 토큰을 포함하여 로그인 구현 </li>
<li> 로그아웃 버튼 클릭 시 handleLogout 함수 실행</li>
<li> mousedown 이벤트가 발생했을 때 NavMenu가 오픈되도록 이벤트 리스너 등록</li>


| Header |
| :---: |
| ![header](https://github.com/Ticketpong/.github/assets/154482912/7ca4663b-0e14-472a-acc5-7e5f777a167c) |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

#### []

<li></li>
<li></li>
<li></li>

|      |
| :---: |
|      |

<hr>

### 7. 개선 목표

<hr>

### 8. 프로젝트 후기
