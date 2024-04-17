![main](https://github.com/Ticketpong/.github/assets/154482912/fa4a1591-3841-42ca-988b-f41b2581b9ea)
<br/>
<br/>
<div>
<h3>프로젝트 소개</h3>
  <li> 티켓 예매 사이트 티켓퐁은 독점 방지를 위한 예매사이트 분산의 필요성과 소비자 편의성 제공을 목적으로 시작했습니다. </li>
  <li> 문화생활에 대한 접근성을 높일 수 있는 정보 집약적 서비스 구현을 목표로 하고 있습니다.</li>
  <li> 카드별 할인 혜택을 제공하는 결제 구조를 구현했습니다..</li>
  <li> 위치기반 서비스로 지역별 공연 마케팅 효과를 만들고자 했습니다.</li>
  <li> 안전한 예매를 위한 사용자 인증 기기 등록이 가능합니다.</li>
</div>
<br/>
<hr>

### 팀원 구성
| 황인식 | 손지연 |  박우정   |  이예리  |  양재식   |  송운정   |
| :--------: | :--------: | :------: | :-----: | :-----: | :-----: |
|  조장 |   백엔드    | 백엔드 | 프론트 | 프론트 | 프론트 |

<br/>
<hr>


### 1. 개발 환경</h3>

  #### Front
  |Java | HTML|CSS3 | React| 
  |:----:|:----:|:-----:|:-:|
  |![Java](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=JavaScript&logoColor=white) | ![html](https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=whit) | ![css](https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=whit) | ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB) |
  
#### Back-end
  |Node.js | MySQL|MariaDB | Express.js| 
  |:----:|:----:|:-----:|:-:|
  |![](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white) | ![html](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white) | ![css](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white) | ![React](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge) |

  #### 협업툴
  |Vscode | Zoom| Github | Figma| 
  |:----:|:----:|:-----:|:-:|
  |![](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white) | ![](https://img.shields.io/badge/Zoom-2D8CFF?style=for-the-badge&logo=zoom&logoColor=white) | ![](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white) | ![](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white) |
  
<br/>
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
  <li>Feat 브랜치는 기능 단위로 독립적인 개발 환경을 위하여 사용하고 merge 후, 각 브랜치를 삭제해주었습니다.</li>
</div>
<br/>
<hr>
  
### 3. ERD
![ERD](https://github.com/Ticketpong/.github/assets/154482912/68d0de05-7ffc-45e5-b1d4-fcdac9164435)

<br/>
<hr>

### 4.  프로젝트 구조

#### Front

- README.md
- src
   - App.css
   - App.js
   - assets
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
<br/>
<hr>

### 5.  역할 분담

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
<br/>
<hr>

### 6.  개발 기간 및 작업 관리
![time](https://github.com/Ticketpong/.github/assets/154482912/b20a5c0f-50e5-4f90-8745-360ec59f9f05)

<br/>
<hr>

#### 작업 관리

<li>Zoom을 이용해서 실시간 소통을 하면서 상황을 공유하며 진행했습니다.</li>
<li>Git-flow 전략을 기반으로 main, feature, develop 브랜치를 운용했습니다. </li>
<br/>
<hr>

### 7. 기능 설명

#### [Header]
<li> useEffect와 axiosWithAuth를 이용, 사용자 인증 토큰을 포함하여 로그인 구현 </li>
<li> 로그아웃 버튼 클릭 시 handleLogout 함수 실행</li>
<li> mousedown 이벤트가 발생했을 때 NavMenu가 오픈되도록 이벤트 리스너 등록</li>


| Header |
| :---: |
| ![header](https://github.com/Ticketpong/.github/assets/154482912/7ca4663b-0e14-472a-acc5-7e5f777a167c) |

<br/>

#### [배너 슬라이더]

<li> isActive와 setInterval을 이용하여 이미지 페이드 효과 구현</li>
<li> 검색어 입력시 keyword가 업데이트되며 엔터/아이콘 클릭 시 handleSearch 함수 호출</li>
<li> fetch 함수를 사용하여 서버에 요청을 보낸 후 response.json으로 변환</li>

|  배너 슬라이더    |
| :---: |
|   ![회원가입](https://github.com/Ticketpong/.github/assets/154482912/ff661e1e-e8f6-4402-8a2e-c438f369d2e0)

   <br/>

#### [카테고리 슬라이더]

<li> 모든 데이터는 useEffect와 axios를 통해 MariaDB에 연결하여, URL을 통해 출력</li>
<li> 데이터 내부에서 카테고리를 가져왔을때, getdisplayedData 함수를 통해 버튼별로 분류</li>
<li> categoryButton이 눌릴 때, hadleCategoryChange 함수를 실행하며, 분류별로 출력</li>

|   카테고리 슬라이더   |
| :---: |
|   ![카테고리배너](https://github.com/Ticketpong/.github/assets/154482912/0f4b559f-0e3a-413c-a90c-0dfa3b9a9a3a)

   <br/>

#### [Login]

<li> useState와 axios로 로그인 내용을 backend로 전달</li>
<li> 로그인 버튼 클릭시 backend 전송후 성공 시 token을 생성</li>
<li> Token 생성후 localStorage에 isLogined, userId을 토큰으로 저장</li>

|   Login   |
| :---: |
|    ![로그인](https://github.com/Ticketpong/.github/assets/154482912/bff53e6d-3571-4df7-b1d0-030bc62c2624)

  <br/>

#### [Sign up]

<li> useState로 변경변수, 주소검색창, 아이디, 이메일 체크 되도록 구현</li>
<li> react-daum-posstcode로 주소 검색 구현</li>
<li> 아이디/이메일 확인을 axios로 체크한 뒤, 회원가입이 가능하도록 구현</li>

|    Sign up  |
| :---: |
|   ![회원가입(수정)](https://github.com/Ticketpong/.github/assets/154482912/01a9ebf1-cbab-40dc-950e-33d26a4e8216)

   <br/>

#### [ID/PW 찾기]

<li> useState로 변수 설정</li>
<li> axios로 백엔드와 연결 후 결과값 반환  </li>
<li> 결과값을 useNavigate로 페이지 이동과 함께 state로 결과값 전달 </li>
<li> 전달받은 값은 useLocation로 받아와 변수에 저장</li>

|   ID/PW 찾기   |
| :---: |
|   ![아이디_비밀번호 찾기](https://github.com/Ticketpong/.github/assets/154482912/39bb0dd7-8b14-49f8-9e6a-736054cbd8f9)

   <br/>

#### [Boxoffice Ranking]

<li> 모든 데이터는 useEffect와 axios를 통해 MariaDB에 연결하여, URL을 통해 출력</li>
<li> 박스오피스 순위 테이블을 가져와서, 순위별로 순서대로 출력</li>

|   Boxoffice Ranking   |
| :---: |
|     |

<br/>

#### [전체 공연 카테고리]

<li> 위치기반 필터링을 활성화하여 handleGeographyChange 함수를 호출</li>
<li> 현재 사용자의 위치 정보(위도, 경도)를 가져오기 위해 브라우저의 geolocation API를 이용</li>
<li> 선택한 카테고리에 따라 공연을 필터링하여 getDisplayedData 함수 호출</li>
<li> 위치정보 버튼을 누를 경우, 위치 액세스를 할 경우, 사용자 주변 반경 11km 범위의 데이터를 제공</li>
<li> 공연 데이터를 선택한 기준에 따라 보여주는 filteredData를 출력</li>

|   전체 공연 카테고리   |
| :---: |
|   ![공연 카테고리](https://github.com/Ticketpong/.github/assets/154482912/558a3b04-b417-467f-a215-24c32fab6aa8)

   <br/>

#### [더보기 및 데이터 정렬]

<li> 출력하는 데이터의 갯수를 제한해놓고, 더보기버튼을 누르면 handelLoadMore 함수를 실행</li>
<li> 출력된 모든 데이터들은 handleSortBy 함수에 의해 가나다, 최근 등록순, 종료일 늦은 순으로 정렬 </li>


|   더보기 및 데이터 졍렬   |
| :---: |
|   ![더보기 및 데이터 정렬](https://github.com/Ticketpong/.github/assets/154482912/ff306dff-8807-40e6-b413-4487441544b4)

   <br/>

#### [공연 스케줄 처리]

<li> 예시와 같은 데이터가 들어오면 각 요일과 시간으로 분리 </li>
<li> 날짜 범위가 ‘~’ 로 표기된 경우 인덱스 차이를 이용해 요일 설정</li>
<li> 괄호 내부 시간 데이터 추출</li>

|   공연 스케줄 처리   |
| :---: |
|   ![1 공연 스케줄 처리](https://github.com/Ticketpong/.github/assets/154482912/b1c4f393-108f-49ef-9eed-469d78a33f2b)
   
<br/>

#### [좌석 선택 및 예매]

<li> 불러온 공연 데이터 기반 예매 가능 날짜와 시간 설정 </li>
<li> 기존 예매자 회원정보 데이터와 카드 할인율 반영하여 결제 요청</li>
<li> 결제 요청 성공시 콜백 함수 실행하여 DB에 예매 정보 저장</li>

|   좌석 선택 및 예매   |
| :---: |
|   ![2 좌석 선택 및 예매](https://github.com/Ticketpong/.github/assets/154482912/3f238424-9fc1-4b1e-bfe5-184b6ce6cc71)
   

<br/>

#### [예매 기기 미등록/ 불일치 시]

<li>- 등록된 기기와 접속한 기기 불일치 시 예매 불가</li>
<li>- 기기 미등록 시 기기 등록 페이지로 이동 후 기기 등록
  (30일 이후 재등록 가능)</li>

|   예매 기기 미등록/불일치 시   |
| :---: |
|   ![3 예매(기기 미등록)](https://github.com/Ticketpong/.github/assets/154482912/9e25db65-274e-4c25-85ec-7cec4df5f6f2)

   <br/>

#### [공연 상세페이지]

<li> 각 탭별 인덱스 부여 </li>
<li> 해당 공연의 리뷰 데이터 호출</li>
<li> 해당 공연의 공연 시설 위도, 경도 추출하여 지도 표시 및 길찾기 기능 지원</li>

|    공연 상세페이지  |
| :---: |
|   ![4 공연 상세페이지 탭](https://github.com/Ticketpong/.github/assets/154482912/092a66df-d2ff-4ca9-8506-eacc16936ac5)

<br/>

##### [커뮤니티]


<li> 공지사항 게시판, 리뷰 전체, 이용사항 안내 조회 가능</li>
<li> URL을 통해 리뷰 데이터 테이블에 연결하여 추천수, 별점, 리뷰 내용을 출력</li>
<li> 본인이 등록한 리뷰 CRUD 가능  </li>
<li> recommandHandler 함수를 통해 로그인되어 있다면, 추천을 줄 수 있음</li>

|   커뮤니티  |
| :---: |
| ![커뮤니티](https://github.com/Ticketpong/.github/assets/154482912/8ef87721-d1cc-4d45-99fd-3da10f8c25a4)

 <br/>

##### [예매 내역]


<li> 해당 유저의 예매 데이터를 서버에서 가져와 렌더링</li>
<li> 예매 취소 시 오늘 날짜와 예매한 공연 날짜 비교 후 관람일 이전에만 취소 가능</li>
<li> 이미 결제 취소 되거나 취소 불가한 경우 처리</li>

|   예매 내역  |
| :---: |
| ![5 예매 내역 확인 및 취소](https://github.com/Ticketpong/.github/assets/154482912/b8e39982-a3dc-47a7-a130-3d7d81150e7b)
 
<br/>

##### [후기 작성]


<li> 관람일 이후 후기가 작성 되지 않았을 경우에만 작성 가능</li>
<li> 해당 유저가 작성한 리뷰 데이터 인덱싱하여 각 리뷰별 렌더링</li>

|   후기 작성  |
| :---: |
| ![6 예매 후기 작성](https://github.com/Ticketpong/.github/assets/154482912/088151d7-6047-4e5b-898e-ae9a61fd2fdf)
 

<br/>

##### [회원정보수정]


<li> useState로 변경되는 변수를 설정</li>
<li> useEffect, axiosWithAuth함수를 이용하여 Token값 가져오기</li>
<li> axiosWithAuth는 localStorage에 있는 Token값을 받아와 decode 하는 함수</li>

|  회원정보수정   |
| :---: |
| ![회원정보수정(수정)](https://github.com/Ticketpong/.github/assets/154482912/1dd3db45-6d13-4bf6-90ed-badc492285cf)
 
<br/>

##### [회원정보수정2]


<li> useState로 변경되는 변수를 설정</li>
<li> useEffect, axiosWithAuth함수를 이용하여 Token값 가져오기</li>
<li> 비밀번호를 입력받아 backend로 전달, 처리 값 받기</li>
<li> true일 경우에만 수정페이지로 id값과 함께 이동하도록 구현</li>

|  회원정보수정2   |
| :---: |
| ![회원정보수정(수정)](https://github.com/Ticketpong/.github/assets/154482912/62dd4f63-952c-4c62-8b97-d157534e7246)

 <br/>

##### [회원정보수정3]

<li> useState로 변경되는 변수를 설정</li>
<li> useEffect, axios로 backend에서 id별 정보를 가져와 저장</li>
<li> value 값에 나와야 하는 값들의 변수를 넣어 화면에 출력되도록 구현</li>
<li> 삭제, 수정 버튼을 누르면 그 값들이 backend로 넘어가 처리되도록 구현</li>

|  회원정보수정3   |
| :---: |
| ![회원정보수정(수정)](https://github.com/Ticketpong/.github/assets/154482912/37ecfbb1-091c-468a-a252-6240328e1282)


 <br/>

##### [회원관리 화면 & Paging]


<li> useEffect와 axiosWithAuth를 이용하여 로그인 핸들링</li>
<li> 회원 정보 리스트  출력</li>
<li> ITEMS_PER_PAGE 상수로 사용하여 데이터를 페이지별로 렌더링</li>

|   회원관리 화면 & Paging  |
| :---: |
|  |

<br/>

##### [공연 관리 리스트]


<li> useState 훅을 사용하여 현재 페이지(currentPage)와 데이터를 관리</li>
<li> fetchData 함수를 호출하여 서버에서 공연 데이터를 가져옴</li>


|   공연 관리 리스트  |
| :---: |
|  |

<br/>

##### [공연 등록 화면]


<li> 사용자가 "완료" 버튼을 클릭했을 때 submit 함수가 실행</li>
<li></li>
<li></li>


|   공연 등록 화면  |
| :---: |
|  |

<br/>

##### [회원관리화면 & Paging]


<li> map 함수를 사용하여 각 리뷰를 ReviewItem 컴포넌트로 렌더링</li>
<li> fetchData 함수로 최근 리뷰 목록을 가져옴</li>
<li> goToPrevPage, goToNextPage 함수 사용해서 페이징 처리</li>

|   회원관리화면 & Paging  |
| :---: |
|  |
<br/>
<hr>

### 8. 프로젝트 후기
