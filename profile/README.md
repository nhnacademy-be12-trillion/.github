# Trillion 📖

> trillion-book 온라인 서점

### Trillion 도메인
[Trillion](http://trillion-book.shop/)

## 📜 목차
- [🗓️ 프로젝트 개요](#%EF%B8%8F-프로젝트-개요)
    - [진행 기간](#진행-기간)
    - [팀 구성](#팀-구성-)
- [서비스 소개](#-서비스-소개)
- [서비스 설계](#-서비스-설계)
    - [기술 스택](#기술-스택)
    - [ERD](#erd)
    - [Architecture](#architecture)
    - [Docs](#docs)
- [기능 소개](#-기능-소개)
- [느낀점](#-느낀점)

## 🗓️ 프로젝트 개요

### 진행 기간

- 2025.11.11 ~ 2025.12.31 (8주)
  <br>

## 팀 구성
|             [강병호](https://github.com/Splleat)              |             [김세현](https://github.com/byesummer)              |             [김근오](https://github.com/roben0510)              |             [박성호](https://github.com/serrot24)              |
|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|
| <img width="130px" src="https://github.com/Splleat.png" /> | <img width="130px" src="https://github.com/byesummer.png" /> | <img width="130px" src="https://github.com/roben0510.png" /> | <img width="130px" src="https://github.com/serrot24.png" /> |
|                          주문 서비스                          |                          회원 서비스                          |                          검색 서비스                          |                         인프라 서비스                         |

|             [이승현](https://github.com/SHYiii)              |             [정현수](https://github.com/hyunsu15)              |             [조은해](https://github.com/eee88)              |             [최지훈](https://github.com/ChousnCom)              |
|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|:----------------------------------------------------------:|
| <img width="130px" src="https://github.com/SHYiii.png" /> | <img width="130px" src="https://github.com/hyunsu15.png" /> | <img width="130px" src="https://github.com/eee88.png" /> | <img width="130px" src="https://github.com/ChousnCom.png" /> |
|                         장바구니 서비스                         |                          쿠폰 서비스                          |                          도서 서비스                          |                          결제 서비스                          |

<br>

## 📢 서비스 소개
[📎 YouTube Link](유튜브_시연영상_링크_입력)

<br>

## 서비스 설계
### 기술 스택

#### **Backend**
<img src="https://img.shields.io/badge/java 21-007396?style=for-the-badge&logo=java&logoColor=white"> <img src="https://img.shields.io/badge/spring boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"> <img src="https://img.shields.io/badge/spring security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white"> <img src="https://img.shields.io/badge/spring jpa-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
<br>
<img src="https://img.shields.io/badge/spring cloud gateway-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/spring eureka-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/spring openfeign-6DB33F?style=for-the-badge&logo=spring&logoColor=white"> <img src="https://img.shields.io/badge/spring config-6DB33F?style=for-the-badge&logo=spring&logoColor=white">
<br>
<img src="https://img.shields.io/badge/maven-C71A36?style=for-the-badge&logo=maven&logoColor=white"> <img src="https://img.shields.io/badge/jwt-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"> <img src="https://img.shields.io/badge/swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"> <img src="https://img.shields.io/badge/lombok-BC0230?style=for-the-badge&logo=lombok&logoColor=white">

#### **Frontend**
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> <img src="https://img.shields.io/badge/css3-1572B6?style=for-the-badge&logo=css3&logoColor=white"> <img src="https://img.shields.io/badge/thymeleaf-005F0F?style=for-the-badge&logo=thymeleaf&logoColor=white">

#### **Database & Cache**
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> <img src="https://img.shields.io/badge/redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"> <img src="https://img.shields.io/badge/h2-003B57?style=for-the-badge&logo=h2&logoColor=white">

#### **Infrastructure**
<img src="https://img.shields.io/badge/github actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"> <img src="https://img.shields.io/badge/docker compose-2496ED?style=for-the-badge&logo=docker&logoColor=white"> <img src="https://img.shields.io/badge/nginx-009639?style=for-the-badge&logo=nginx&logoColor=white"> <img src="https://img.shields.io/badge/minio-C72C48?style=for-the-badge&logo=minio&logoColor=white"> <img src="https://img.shields.io/badge/elasticsearch-005571?style=for-the-badge&logo=elasticsearch&logoColor=white">

#### **Tools & Collaboration**
<img src="https://img.shields.io/badge/sonarqube-4E9BCD?style=for-the-badge&logo=sonarqube&logoColor=white"> <img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white"> <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/notion-000000?style=for-the-badge&logo=notion&logoColor=white"> <img src="https://img.shields.io/badge/dooray!-262B40?style=for-the-badge">

### ERD
<img width="100%" alt="Trillion ERD" src="./images/trillion-erd.png" />

### Architecture
<img width="100%" alt="Trillion Architecture" src="./images/architecture.png" />

### Docs
[Trillion Team Wiki](https://github.com/nhnacademy-be12-trillion/project_wiki/wiki)

<br>

## 기능 소개

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
- 담당자 : 조은해, 최지훈
    - 도서 등록, 수정, 조회 (CRUD) 구현
    - 주문량, 조회수, 카테고리별 도서 정렬 기능 구현
    - 알라딘 Open API 기반 도서 데이터 수집 및 보강
    - Gemini API를 활용한 도서 데이터 보강 기능 구현
    - CSV 파일을 파싱하여 도서 데이터 일괄 등록 구현

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
    - 회원/비회원 장바구니 CRUD(상품 추가, 수량 변경, 삭제) 기능 구현
    - 성능을 위해 Redis를 활용하여 장바구니 기능을 구축하고, 회원 데이터는 DB에 영구 저장하여 안정성 확보
    - 모든 장바구니 연산을 Redis(In-Memory)에서 처리하여 응답 지연(Latency) 최소화
    - Write-Back(지연 쓰기) 패턴을 적용, 스케줄러를 통해 Redis 데이터를 DB에 비동기 동기화하여 영속성 보장
    - 데이터 생명주기 관리 및 리소스 최적화를 위해 담은 지 90일 경과 상품 자동 삭제 스케줄러 구현

### **📱 주문**
- 담당자 : 강병호
    - Orchestration Saga 패턴 기반의 주문 생성 및 취소, 환불 분산 트랜잭션 구현
    - 스케줄러를 이용한 중단된 트랜잭션 복구 시스템 구축
    - 멱등성 키 설계를 통한 중복 요청 방어 및 데이터 정합성 확보
    - 배송 정책 및 포장지 관리 등 주문 관련 부가 도메인 기능 구현

### **💳 결제**
- 담당자 : 최지훈
    - TossPayments API와 연동.
    - 결제 승인/실패 프로세스

### **📝 리뷰**
- 담당자 : 김근오, 조은해
    - 리뷰 조회, 등록, 수정 기능 구현
    - AI 모델을 활용한 리뷰 요약 기능 구현

### **❤️ 위시리스트**
- 담당자 : 조은해
    - 위시리스트(관심 상품) 등록, 조회, 삭제 (CRUD) 구현

### **🚚 배송 / 📦 포장지**
- 담당자 : (담당자 이름)
    - 배송비 정책 관리
    - 선물 포장 옵션 선택 기능

### **📂 파일**
- 담당자 : 조은해
    - MinIO Object Storage를 이용한 도서 및 리뷰 이미지 저장/호출 처리

### **📂 카테고리**
- 담당자 : 조은해, 최지훈
    - 도서 카테고리 매핑 및 구조 관리
    - 카테고리별 도서 목록 조회 기능 구현

### **🔄 배치**
- 담당자 : 정현수
    - 생일쿠폰 발급
    - 비활성화유저 지정
    - 회원등급관리 

<br>

## 느낀점

<table border="1" cellspacing="0" cellpadding="10">
  <tr>
    <th rowspan="3">
      <a href="https://github.com/Splleat">강병호</a><br />
      <img width="130px" src="https://github.com/Splleat.png" /><br />
      주문 서비스
    </th>
    <td colspan="2" rowspan="3">이번 프로젝트를 진행하면서 가장 까다로웠던 점은 여러 서비스에 걸친 트랜잭션의 원자성을 @Transactional 어노테이션만으로 처리할 수 없다는 것이었습니다. 첫 MSA 환경인 만큼 서비스 간 통신과 데이터 정합성 보장 문제를 직접 마주해야 했고, 분산 트랜잭션 과정에서 발생할 수 있는 다양한 예외 케이스들에 대해 고민하여 해결해나가는 과정에서 한 단계 더 성장할 수 있었던 소중한 경험이었습니다.</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/byesummer">김세현</a><br />
      <img width="130px" src="https://github.com/byesummer.png" /><br />
      회원 서비스
    </th>
    <td colspan="2" rowspan="3">(김세현님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/roben0510">김근오</a><br />
      <img width="130px" src="https://github.com/roben0510.png" /><br />
      검색 서비스
    </th>
    <td colspan="2" rowspan="3">(김근오님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/serrot24">박성호</a><br />
      <img width="130px" src="https://github.com/serrot24.png" /><br />
      인프라
    </th>
    <td colspan="2" rowspan="3">(박성호님의 느낀점을 입력해주세요.)</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/SHYiii">이승현</a><br />
      <img width="130px" src="https://github.com/SHYiii.png" /><br />
      장바구니 서비스
    </th>
    <td colspan="2" rowspan="3">처음에는 간단해 보였던 장바구니가 Redis와 RDB 사이의 데이터 동기화 문제를 만나면서 프로젝트 내내 가장 집요하게 파고든 기능이 되었습니다. 조회 성능을 높이기 위해 캐싱을 도입하는 과정에서
        '속도'와 '데이터 정합성' 사이의 trade-off를 끊임없이 고민해야 했고, 이 과정이 꽤나 고통스러웠지만 덕분에 백엔드 개발자의 진짜 재미를 느낄 수 있었습니다. 작은 기능 하나라도 깊이 있게 고민하고 해결했을 때 비로소 내 것이 된다는 걸 배운 소중한 시간이었습니다.</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/hyunsu15">정현수</a><br />
      <img width="130px" src="https://github.com/hyunsu15.png" /><br />
      쿠폰 서비스
    </th>
    <td colspan="2" rowspan="3">팀원을 잘 만나서 무사히 프로젝트를 마무리할 수 있었습니다. 특히 재미있게 팀 분위기를 이끈 3인방에게 감사합니다.</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/eee88">조은해</a><br />
      <img width="130px" src="https://github.com/eee88.png" /><br />
      도서 서비스
    </th>
    <td colspan="2" rowspan="3">이번 프로젝트의 가장 큰 과제는 '방대한 도서 데이터를 어떻게 효율적으로 관리할 것인가'였습니다. 이를 해결하기 위해 초기 데이터 구축 단계에서 CSV 파일을 파싱 하여 DB에 적재하는 기능을 구현했고, 이 과정에서 대량의 데이터를 안정적으로 처리하기 위한 로직을 깊게 고민했습니다.

또한 프로젝트의 핵심인 도서와 리뷰 도메인의 비즈니스 로직을 설계하고, MinIO를 도입해 파일 처리를 구현하며 백엔드 개발의 기술적 역량을 키웠습니다. 무엇보다 팀원들과 호흡을 맞추며, 혼자 개발할 때는 배울 수 없었던 API 설계의 표준화와 코드 일관성이 유지보수에 얼마나 중요한지 깨달을 수 있었던 값진 경험이었습니다.</td>
  </tr>
  <tr></tr>
  <tr></tr>

  <tr>
    <th rowspan="3">
      <a href="https://github.com/ChousnCom">최지훈</a><br />
      <img width="130px" src="https://github.com/ChousnCom.png" /><br />
      결제 서비스
    </th>
    <td colspan="2" rowspan="3">비록 테스트 환경이었지만, 결제는 사용자의 자산과 직결된 서비스의 가장 민감한 영역이기에 실제 상용 서비스라는 마음가짐으로 임했습니다. 외부 PG사와의 통신 과정에서 발생할 수 있는 네트워크 오류나 데이터 불일치 등 모든 예외 상황을 집요하게 시뮬레이션하며 방어 로직을 구축했습니다. 이 과정을 통해 단순히 기능이 동작하는 것을 넘어, '신뢰할 수 있는 시스템'을 만드는 개발자의 책임감을 깊이 배울 수 있었습니다.</td>
  </tr>
  <tr></tr>
  <tr></tr>
</table>
