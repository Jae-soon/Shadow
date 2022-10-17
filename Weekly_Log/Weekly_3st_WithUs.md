## 팀 구성원, 개인 별 역할

<br>

### 금주부터 진행 중인 **개인별 역할** <br>
이번주 개인별로 담당한 부분입니다.입니다. <br><br>

### 🙂권재순

- 역할 : Spring 서버와 CLOVA 연동, DB 캐싱
- 세부 작업 : WebSocket을 사용하여 Spring 서버에서 받은 요청 메세지를 CLOVA를 통해 Keyword 도출, DB 캐싱

### 🙂김동현

- 역할 : 챗봇 UI 수정, 챗봇 통신 방식 변경
- 세부 작업 : 챗봇 ui 수정, 챗봇 socket 방식을 ajax로 변경

### 🙂김예진

- 역할 : 로그인, 로그아웃, 회원가입 수정
- 세부 작업 : 아이디, 이메일 중복체크, 중복체크여부 확인추가, 내부 로직 ajax로 변경

### 🙂박민준

- 역할 : Spring 서버와 CLOVA 연동
- 세부 작업 : WebSocket을 사용하여 Spring 서버에서 받은 요청 메세지를 CLOVA를 통해 Keyword 도출

### 🙂이지원

- 역할 : 챗봇 UI 수정
- 세부 작업 : 버튼 수정, 채팅창 화면 하단 배치, 스크롤을 따라다니는 플로팅 기능 추가
<br>

<br>


### 다음주부터 진행 예정인 **개인별 역할** <br>
다음주 개인별로 담당할 부분입니다. <br><br>

### 🙂권재순

- 역할 : Spring 서버와 DB 연동
- 세부 작업 : CLOVA를 통해 도출한 Keyword를 사용해 DB에 저장 순서도 도출

### 🙂김동현

- 역할 : 내부 서버 홈페이지 UI 구성
- 세부 작업 : 전체 홈페이지 틀 만들기

### 🙂김예진

- 역할 : 내부 서버 홈페이지 UI 구성
- 세부 작업 : 네비게이션 바, 카테고리 바 생성

### 🙂박민준

- 역할 : Spring 서버와 CLOVA 연동
- 세부 작업 : 연동에 대한 전반적인 이해, CLOVA를 통해 도출한 Keyword 쇼핑몰

### 🙂이지원

- 역할 : 내부 서버 홈페이지 구현 
- 세부 작업 :  미정

<br>

## 팀 내부 회의 진행 회차 및 일자


이번주 팀회의 진행 결과는 아래와 같습니다. 총 “**2회차**”의 회의에 **전원 모두** 참석하였습니다.

<details>
<summary> 13회차 (2022.08.16), 디코 음성 채널 진행, 전원 참석</summary>
   <div>  개발과정 공유 0차, 작업일정 수정, branch 생성 및 기능이름 지정 </div>
</details> 
<details>
<summary> 14회차 (2022.08.18), 디코 음성 채널 진행, 전원 참석</summary>
   <div>  개발과정 공유 1차, 문제점 분석 - 강사님 피드백 </div>
</details> 

<br>

## 현재까지 개발 과정 요약


이번주 개발 과정은 

1순위 기능 개발 -> 1차 진행상황 공유 및 merge

### 1순위 기능 개발 -> 1차 진행상황 공유 및 merge
으로 진행 중에 있습니다.


아래는 현재까지의 과정에서 기술적으로 새로 알게된 점과, 어려웠던 점 아쉬웠던 점입니다.  

<br>

### 🙂기술적으로 새로 알게된 점
- HTML Onclick event에서 기본적으로 this를 넘기면 form그 자체지만, event를 넘기면, 이벤트를 발생한 그 주체가 들어간다.
- e.preventDefault를 통해서 submit시 재 랜더링을 막을 수 있지만, 폼 그자체 this를 인자로 넘길 시 재랜더링이되고, event를 넘겨야 구동된다.
- DB 캐싱을 통해 API호출을 줄여 부과되는 요금을 줄일 수 있다. 
- position:fixed 속성 사용시 스크롤을 움직여도 화면 하단에 계속 고정시킬 수 있다.
- ReustEntity 클래스를 이용한 REST API 의 사용을 알게되었고, restponsebody로 보낼때, "html :: #id" 형식을 이용하면 HTML의 값을 data로 보낼 수 있다.
- 일반적인 회원 폼에 필요한 제약조건을 ajax로 동적으로 표현함을 알게 되었다.
<br>

### 😥어려웠던 점
- 모든 페이지에 chatbot을 띄우기 위한 방법을 모색 중 layout, header, footer와 같이 공용으로 처리하는 부분에 script 태그를 통해 삽입하여 해결이 가능해 보이긴 하지만, js 외부 파일 파싱에 대한 공부가 필요해 보인다.
- UI를 변형하여 꾸미는게 힘들다...ㅜ
- 처음 만들때 전체적인 프로젝트의 구조를 떠올려야 하는 것이 힘들다.
<br>

### 😥아쉬운 점
- Java와 JavaScript에 대한 숙련도가 부족해 코드 분석이 쉽게 되지 않아 아쉬웠다. API 구성이 어떻게 되어 있는지 쉽게 분석할 수 있었다면 진전이 조금 더 빨랐지 않았을까..?
- 디자인 감각을 키우고 싶어요 .. 완성도 높게 보이려면 UI도 무시할 수 없겠다는 생각을 했습니당
- IntelliJ에서 js 를 지원해주었으면 좋겠다. 오타가 자주 나서 너무 불편하다.
<br>




## 개발 과정에서 나왔던 질문


### 🤔회의 별 질문 및 내용

이번주 2회차의 회의 중에 나왔던 질문, 회의내용 모음입니다.  
매 회의마다 많은 질문이 오고가고, 서로의 의견을 취합하여 다음 과정을 밟아가고 있습니다.
<br>


### Q1. 0차 진행상황 공유 내용 
<details>
<summary> 세부 내용 </summary>
<div>  

1. clova 연동(재순,민준) : 24일까지 연장 - 24일까지 각자 작업 후, 추후 병합  

2. 기본 채팅 기능(지원,동현) : 18일까지 - branch 생성 : feature-chat  

3. 회원가입/로그인(예진) : 18일까지  

</div>
</details> 

### Q2. 1차 진행상황 공유 내용
<details>
<summary> 세부 내용 </summary>
<div>

1. 예진 : 금주까지 회원정보 수정, 로그인 UI 수정 , master 합칠 준비  
   
2. 동현, 지원 : 금주까지 UI 위치 오른쪽 하단으로 변경, 그외 UI 수정, 모든 서비스에 플로팅하는 방식 구현, clova 와 합칠 준비  

3. 재순, 민준 : 전체적인 소스 이해, 이해한 부분 주석처리 완료, 샘플데이터 (키워드 3개정도) 추가, 금주까지 default chat과 합칠 준비  

</div>
</details>



<br>

### 🤔해결되지 않은 질문 리스트

이번주 어려웠던 점에 대해 강사님 피드백을 받아 1차 해결책을 얻은 부분입니다.


### Q3. 추가 질문 모음 - 강사님 피드백
<details>
<summary> 세부 내용 </summary>
<div>

## 문제점 및 개선사항
1. 불필요하게 과다한 스펙으로 웹소켓이 사용됨 -> ajax 로 변경 
2. API 횟수를 줄이기 위해서 (건별로 돈이 나가기 때문에) DB에 데이터를 저장하는 API 캐싱 기능을 추가


## 기존 구조  vs 수정된 구조 ##
크게 3가지 상황으로 나누었습니다.

1. 클라이언트 (사용자) 가 "반품이뭐야" 라고 데이터를 보냄
기존 : 사용자 메세지 입력폼(타임리프) --> 웹소켓(방식) --> 스프링 서버
수정 : 사용자 메세지 입력폼(타임리프) --> ajax(방식) --> 스프링 서버

2. 서버 (스프링서버) 가 clova로 부터 "반품" 이라고 키워드를 받음
기존: 스프링 -- findMsg "반품이뭐야" -->  웹소켓(방식) --> clova -- "반품" --> 스프링
수정: 스프링 -- findMsg "반품이뭐야" --> DB -- false --> 스프링 -- 웹소켓(방식) --> clova -- "반품" --> 스프링 -- msg="반품이뭐야", keyword="반품" --> DB

3. 서버(스프링서버) 가 "반품"의 에 대한 "순서도"도 데이터를 클라이언트에게 보냄
기존: 스프링 서버 -- findFlow "반품" --> DB -- 반품순서도 --> 스프링 서버 -- 웹소켓(방식)--> 사용자 메세지 출력 (타임리프)
수정: 스프링 서버 -- findFlow "반품" --> DB -- 반품순서도 --> 스프링 서버 -- ajax(방식) --> 사용자 메세지 출력 (타임리프)

## 상세 수정된 구조 ##
크게 3가지 상황으로 나누었습니다.

1. 클라이언트 (사용자) 가 "반품이뭐야" 라고 데이터를 보냄
사용자 메세지 입력폼(타임리프) --> ajax(방식) --> 스프링 서버

2. 서버 (스프링서버) 가 clova로 부터 "반품" 이라고 키워드를 받음
"반품이뭐야" 라는 입력이 처음 들어온 상황(디비 캐시에 없었음)
스프링 -- findMsg "반품이뭐야" --> DB -- false --> 스프링 -- 웹소켓(방식) --> clova -- "반품" --> 스프링 -- msg="반품이뭐야", keyword="반품" --> DB

    2.1. DB 에 "반품이뭐야" 가 있는지 확인 
    스프링 -- findMsg "반품이뭐야" --> DB

    2.2. DB로부터 "반품이뭐야" 없음을 받고, clova 에 데이터 요청
    DB -- false --> 스프링 -- 웹소켓(방식) --> clova
    (clova와 스프링을 연동할 때, 웹소켓 외에는 레퍼런스가 없어서 현재와 동일하게 웹소켓으로 데이터를 받아옵니다.)

    2.3. clova로 부터 "반품" 이라는 키워드 받아옴
    clova -- "반품" --> 스프링

    2.4. DB 에 "반품이뭐야" (key) "반품" (value) 저장
    스프링 -- msg="반품이뭐야", keyword="반품" --> DB


3. 서버(스프링서버) 가 "반품"의 에 대한 "순서도"도 데이터를 클라이언트에게 보냄
스프링 서버 -- findFlow "반품" --> DB -- 반품순서도 --> 스프링 서버 -- ajax(방식) --> 사용자 메세지 출력 (타임리프)

</div>
</details>

<br>

## 개발 결과물 공유

이번주는 설계도에서 수정된 부분은 없으며, 전체적인 개발 진행 중으로, Github 결과물을 공유드립니다.

### 😀결과물

#### Github Repository URL

[https://github.com/likelion-backendschool/Withus](https://github.com/likelion-backendschool/Withus)


<br>

### 😀WBS
<br>

#### WBS 엑셀
[https://docs.google.com/spreadsheets/d/1mbyUlXgf4MniXAPvGZXqFZ4QALEV3PRuGO6nmig7BFU/edit#gid=0](https://docs.google.com/spreadsheets/d/1mbyUlXgf4MniXAPvGZXqFZ4QALEV3PRuGO6nmig7BFU/edit#gid=0)

<br>

#### 로드맵/진행상황 노션
[https://bold-cardigan-771.notion.site/758df6c483da4c4fb676910e725dca32?v=21e9cd36b03f4558af878e8cc8ec8ff4](https://bold-cardigan-771.notion.site/758df6c483da4c4fb676910e725dca32?v=21e9cd36b03f4558af878e8cc8ec8ff4)

<br>   

### 😀With Us 팀원들의 모습

![3주차 With us 팀원들의 모습](https://i.imgur.com/UDb7DTW.jpg)