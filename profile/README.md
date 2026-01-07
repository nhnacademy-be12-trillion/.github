# Trillion 📖

> trillion-book 온라인 서점

### Trillion 도메인
[📎 Trillion](http://trillion-book.shop/)

## 📜 목차
- [🗓️ 프로젝트 개요](#%EF%B8%8F-프로젝트-개요)
    - [진행 기간](#진행-기간)
    - [팀 구성](#팀-구성-)
- [📢 서비스 소개](#-서비스-소개)
- [🥳 서비스 설계](#-서비스-설계)
    - [기술 스택](#기술-스택)
    - [ERD](#erd)
    - [Architecture](#architecture)
    - [Docs](#docs)
- [🤗 기능 소개](#-기능-소개)
- [😆 느낀점](#-느낀점)

## 🗓️ 프로젝트 개요

### 진행 기간

- 2025.11.11 ~ 2025.12.31 (8주)
  <br>

## 팀 구성 🔥
|             [강병호](https://github.com/Splleat)              |             [김세현](https://github.com/byesummer)              |             [김근오](https://github.com/roben0510)              |             [박성호](https://github.com/serrot24)              |
|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|
| <img width="130px" src="https://github.com/Splleat.png" /> | <img width="130px" src="https://github.com/byesummer.png" /> | <img width="130px" src="https://github.com/roben0510.png" /> | <img width="130px" src="https://github.com/serrot24.png" /> |
|                         주문 서비스                          |                         회원 서비스                          |                         검색 서비스                          |                        인프라 서비스                         |

|             [이승현](https://github.com/SHYiii)              |             [정현수](https://github.com/hyunsu15)              |             [조은해](https://github.com/eee88)              |             [최지훈](https://github.com/ChousnCom)              |
|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|
| <img width="130px" src="https://github.com/SHYiii.png" /> | <img width="130px" src="https://github.com/hyunsu15.png" /> | <img width="130px" src="https://github.com/eee88.png" /> | <img width="130px" src="https://github.com/ChousnCom.png" /> |
|                        장바구니 서비스                         |                         쿠폰 서비스                          |                         도서 서비스                          |                         결제 서비스                          |

<br>

## 📢 서비스 소개
[📎 YouTube Link](유튜브_시연영상_링크_입력)

<br>

## 🥳 서비스 설계
### 기술 스택
### 주요 기술 스택

| **구분** | **Frontend** | **Backend** |
| --- | --- | --- |
| **Language** | HTML, CSS | Java **21** |
| **IDE** | IntelliJ | IntelliJ |
| **Framework** | - | Spring Boot, Spring Security, Spring Web, Spring JPA, Spring Cloud (Gateway, Config, OpenFeign, Eureka), Spring AOP, Spring Session Redis |
| **Library** | - | JWT, Lombok, OpenFeign, Spring Validation, Swagger |
| **Template** | Thymeleaf | - |

### 공통 기술 스택

| **구분** | **기술** |
| --- | --- |
| **DB** | MySQL, Redis, H2 |
| **Infra** | GitHub Action, Docker, Nginx, Elasticsearch, Eureka, Config Server, MinIO |
| **Tools** | GitHub, Notion, Dooray, Wiki |
| **Build** | Maven, Spring Boot, **JaCoCo (Test Coverage)** |
| **Test** | Spring Boot Test, Spring Security, Swagger |

### ERD
[📎 Trillion ERD 구조도](ERD_클라우드_링크_입력)
<img width="100%" alt="Trillion ERD" src="ERD_이미지_경로_입력" />

### Architecture
<img width="100%" alt="Trillion Architecture" src="아키텍처_이미지_경로_입력" />

### Docs
[📎 Trillion Team Wiki](위키_또는_노션_링크_입력)

<br>

## 🤗 기능 소개

### **🏗️ 인프라**
- 담당자 : 박성호
    - Github Action을 활용한 CI/CD 구축
    - Docker-Docker compose 활용 및 Nginx 로드밸런싱/리버스 프록시 설정
    - Gateway, Eureka, ConfigServer 구축
    - 오류 분석을 위한 로그 설계와 EFK-메신저 알림 시트메 구축

### **👤 회원/포인트**
- 담당자 : 김세현
    - 회원 가입, 정보 수정, 탈퇴 등 회원 생애주기 관리
    - 등급별 포인트 적립 및 사용 로직 구현

### **📖 도서**
- 담당자 : 조은해
    - 도서 등록, 수정, 조회 (CRUD) 구현
    - 도서 상세 정보 및 재고 관리 로직

### **🎟️ 쿠폰**
- 담당자 : 정현수
    - 쿠폰 발급, 조회 및 적용 로직 구현
    - 쿠폰 유효성 검증 및 예외 처리

### **🔍 검색**
- 담당자 : 김근오
    - ElasticSearch 기반 도서 검색 기능 구현
    - 검색 성능 최적화

### **🛒 장바구니**
- 담당자 : 이승현
    - Redis-First 전략 : 회원/비회원 장바구니 연산을 전량 Redis에서 처리하여 응답 지연(Latency) 최소화
    - 비동기 영속화 : 스케줄러를 통해 회원의 Redis 데이터를 주기적으로 DB에 동기화하는 Write-Back(지연 쓰기) 패턴 구현
    - 데이터 수면 관리 : 담은지 90일이 경과한 상품을 자동 삭제하는 스케줄러 구현

### **📱 주문**
- 담당자 : 강병호
    - 주문 생성 및 조회 기능 구현
    - 주문 상태 관리 및 배송 추적 시스템

### **💳 결제**
- 담당자 : 최지훈
    - TossPayments API와 연동.
    - 결제 승인/실패 프로세스 

### **📝 리뷰 / ❤️ 좋아요**
- 담당자 : (담당자 이름)
    - 도서 리뷰 작성 및 평점 기능
    - 도서 좋아요 및 관심 상품 등록

### **🚚 배송 / 📦 포장지**
- 담당자 : (담당자 이름)
    - 배송비 정책 관리
    - 선물 포장 옵션 선택 기능

### **📂 파일
- 담당자 : (담당자 이름)
    - MinIo를 이용한 이미지/파일 업로드 및 관리
    - 도서 카테고리 분류 및 계층 구조 관리
 
### **📂 카테고리**

<br>

## 😆 느낀점

<table border="1" cellspacing="0" cellpadding="10">
  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">강병호</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      주문 서비스
    </th>
    <td colspan="2" rowspan="3">(강병호님의 느낀점을 입력해주세요. 프로젝트를 진행하며 겪은 기술적 어려움이나 성장한 점 등을 작성하면 좋습니다.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">김세현</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      회원 서비스
    </th>
    <td colspan="2" rowspan="3">(김세현님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">김근오</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      검색 서비스
    </th>
    <td colspan="2" rowspan="3">(김근오님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">박성호</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      인프라
    </th>
    <td colspan="2" rowspan="3">(박성호님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">이승현</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      장바구니 서비스
    </th>
    <td colspan="2" rowspan="3">(처음에는 간단해 보였던 장바구니가 Redis와 RDB 사이의 데이터 동기화 문제를 만나면서 프로젝트 내내 가장 집요하게 파고든 기능이 되었습니다. 조회 성능을 높이기 위해 캐싱을 도입하는 과정에서
        '속도'와 '데이터 정합성' 사이의 trade-off를 끊임없이 고민해야 했고, 이 과정이 꽤나 고통스러웠지만 덕분에 백엔드 개발자의 진짜 재미를 느낄 수 있었습니다. 작은 기능 하나라도 깊이 있게 고민하고 해결했을 때 비로소 내 것이 된다는 걸 배운 소중한 시간이었습니다.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">정현수</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      쿠폰 서비스
    </th>
    <td colspan="2" rowspan="3">(정현수님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">조은해</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      도서 서비스
    </th>
    <td colspan="2" rowspan="3">(조은해님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/아이디">최지훈</a><br />
      <img width="130px" src="https://github.com/아이디.png" /><br />
      결제 서비스
    </th>
    <td colspan="2" rowspan="3">()</td>
  </tr>
  <tr></tr>
  <tr></tr>
</table>
