### 금융 상품 비교 애플리케이션
#빅뱅크

### 목차
1. 팀원 소개 및 업무 분담 내역
2. 설계 및 구현
3. 데이터베이스 모델링(ERD)
4. 서비스 기능에 대한 설명
5. 느낀점, 후기


## 팀원 소개 및 업무 분담 내역
- 프로젝트 기간 : 2024-05-16 ~ 2024-05-23

|이름|업무 및 구현 |
|---|---|
| 강동형 (팀장) |Front End - CSS 총괄 및 구현, 주변 은행 검색 회원가입, 로그인, 마이페이지, 홈, 금융 상품 비교 페이지 구현, 환율 계산기 페이지 구현, 게시판 CRUD, 상품 관리, |
|박재혁(팀원) |Back End - ERD 다이어그램 작성, 금융상품 저장 및 필터링, 회원정보 커스터마이징, 환율 정보 저장 및 업데이트, 금융 상품 회원 저장, 게시판 CRUD 구현, AI 챗봇 구현 및 추천 알고리즘 구현<br> Front End - 개인프로필, 계약 상품 상세정보 |

## 설계 및 구현
### 기술 스택
* Back
  - Python
  - Django
  - Django-rest-framework
  - dj-rest-auto
  - DRF-spectacular
  - REST-API
  - SQL-Lite

* Front
  - JavaScript
  - Vue3
  - Vueitfy
  - Axios
  - Pina
  - Pina-Plugin-Persistedstate
  - Bootstrap
  - Chart.js

## API 명세서 
<img src='./README_IMG/API.png' alt='ERD 이미지' /> 

## 데이터베이스 모델링(ERD)
[**ERD LINK**](https://dbdiagram.io/d/664ab074f84ecd1d229827ad)
<img src='./README_IMG/ERD.png' alt='ERD 이미지' />

## 기능 설명

### 홈페이지
<img src='./README_IMG/Main.png' alt='Main 이미지' /> 
<img src='./README_IMG/Signup.png' alt='Signup 이미지' /> 
<img src='./README_IMG/AlreadySignup.png' alt='AlreadySignup 이미지' /> 
- BIG BANK의 이름처럼 내 손안에 있는 뱅크 즉, 우주를 뱅크로 비교하였습니다.
- 이를 통해 편리하게 금융 상품을 비교하고, 환율 계산, 주변 은행 검색, 자유 게시판을 통해 편리한 서비스를 제공합니다.
- 또한 CHAT BIGBANK를 이용해 금융 관련 질문이나 나에게 맞는 금융 상품을 소개받을 수 있습니다.

### 마이페이지
<img src='./README_IMG/Profile.png' alt='Profile 이미지' /> 
<img src='./README_IMG/ContractDepositDetail.png' alt='ContractDepositDetail 이미지' /> 
<img src='./README_IMG/ContractSavingDetail.png' alt='ContractSavingDetail 이미지' /> 
- 마이페이지에선 내정보를 확인 하고 수정할 수 있습니다.
- 내가 가입한 적금, 예금에 대해서 확인을 할 수 있으며 클릭하면 상세보기 및 금리, 최고금리를 개월별로 비교할 수 있도록 구현하였습니다.

### 금융 상품 비교 페이지
<img src='./README_IMG/DeopsitSavingList.png' alt='DeopsitSavingList 이미지' /> 
<img src='./README_IMG/DepositDetail.png' alt='DepositDetail 이미지' /> 
<img src='./README_IMG/SavingDetail.png' alt='SavingDetail 이미지' /> 
- 은행별로 예금, 적금 상품을 한눈에 볼 수 있도록 구현하였습니다.
- 또한 상품 클릭시 공시 제출월, 금융회사명, 상품명, 가입제한, 금리, 가입방법, 우대조건 등 상세 정보를 확인 할 수 있습니다.

### 환율 계산 페이지
<img src='./README_IMG/Extrate.png' alt='Extrate 이미지' /> 
- 나라별 원화와 각국의 통화를 비교하며 환율을 파악 할 수 있도록 구현하였습니다.
- 원화를 수정하면 각국의 통화가 바로 나오고, 각국의 통화를 수정하면 원화가 바로 나올 수 있도록 구현하였습니다.

### 주변 은행 검색 페이지
<img src='./README_IMG/BankMap.png' alt='BankMap 이미지' /> 
- 적금 예금 데이터에 저장이 된 은행들을 수도권과 광역시를 기준으로 편리하게 확인을 할 수 있도록 콤보박스로 구현하였습니다.

### 자유 게시판
<img src='./README_IMG/ArticleList.png' alt='ArticleList 이미지' />
<img src='./README_IMG/ArticleCreate.png' alt='ArticleCreate 이미지' />
<img src='./README_IMG/ArticleUpdate.png' alt='ArticleUpdate 이미지' />
<img src='./README_IMG/CommentList.png' alt='CommentList 이미지' />
<img src='./README_IMG/CommentUpdate.png' alt='CommentUpdate 이미지' />
- 게시글을 확인할 수 있고 게시글 작성, 수정, 삭제를 구현하였습니다.
- 댓글기능 또한 리스트와 작성 ,수정, 삭제 기능을 구현하였습니다.
- 본인이 작성한 글과 작성한 댓글에 대해서만 수정 및 삭제를 구현 할 수있도록 하였습니다.

### CHAT BIGBANK
<img src='./README_IMG/ChatBigBank.png' alt='ChatBigBank 이미지' /> 
- 인공지능을 이용한 CHAT BOT을 구현하였습니다.
- 기본적인 일상의 이야기나 금융과 관련한 정보를 얻을 수 있으며 고객들이 편리하게 서비스를 이용 할 수 잇도록 구현하였습니다.

## AI CHAT BANK & 알고리즘
<img src='./README_IMG/Algorithm.png' alt='Algorithm 이미지' /> 
- 알고리즘 같은 경우엔 상품 추천을 부탁하면 AI가 은행과 상품의 형태를 여쭤보는 형식으로 구현하였습니다.
- 이후 은행이름과 상품의 형태 (적금, 예금)를 작성하면 그에 맞는 상품을 제공 합니다.
- 이후 금리가 높은 제품을 추천해달라고하면 데이터셋에 있는 금리가 가장 높은 제품을 제공 할 수  있도록 하였습니다.
친근한 방식으로 문자 메세지를 보내는 듯한 UI를 구현하였습니다.
