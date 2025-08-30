# HeyFy

<img src='https://ifh.cc/g/YRGhBP.jpg' border='0'>


외국인 유학생의 한국 대학 생활 적응을 돕는 **온보딩 서비스 (with 금융)**
> 금융 + 한국 생활 적응 + 커뮤니티를 하나로 연결한 캠퍼스 파트너




<br>

## 👤 팀원 소개
| 박재홍 | 김승상 | 엄유상 | 김해린 | 박대얼 |
|:------:|:------:|:------:|:------:|:------:|
| <a href='https://github.com/prk4224'><img src='https://avatars.githubusercontent.com/u/83493143?v=4' width='100px'/></a> | <a href='https://github.com/seungsang2000'><img src='https://avatars.githubusercontent.com/u/74907427?v=4' width='100px'/></a>  | <a href='https://github.com/EomYoosang'><img src='https://avatars.githubusercontent.com/u/53031768?v=4' width='100px'/></a> | <a href='https://github.com/jenny1zzang'><img src='https://avatars.githubusercontent.com/u/108577676?v=4' width='100px'/></a> | <a href='https://github.com/uioo1'><img src='https://avatars.githubusercontent.com/u/28687099?v=4' width='100px'/></a> |
| 팀장 & FE | BE | BE | BE | AI |

<br>

## 📌 프로젝트 개요
- **프로젝트 명:** HeyFY (헤이파이)  
- **팀 명:** 싸신사 (싸피 + 신한은행 = 사랑)  
- **대상:** 한국 대학 외국인 유학생

<br>

## 💡 기획 배경
- 외국인 유학생 20만 명 시대, 한국 대학 재정과 직결되는 핵심 인구  
- 환율 변동으로 인해 환전 시 경제적 부담 발생
- 비자/문화 적응 문제로 한국 생활에 어려움  
👉 금융 + 생활 + 커뮤니티를 아우르는 온보딩 서비스 필요

<br>

## 🛠 핵심 기능
### 🏦 금융 서비스
- AI 기반 환율 예측 및 환전 추천  
- 등록금 납부 시점 최적화  
- 계좌·카드 추천 및 조회/이체  
- 외국인 등록증 기반 인증 및 금융 접근성 강화  

### 🤝 커뮤니티 & 캠퍼스 적응
- 1:1 멘토링 자동 매칭  
- 맞춤형 동아리 추천  
- 오늘의 캠퍼스 꿀팁 제공  
- 문화·생활 정보 공유 커뮤니티  

### 🧑‍💻 생활 편의
- 비자 유형별 근무 시간 안내 & 알바 추천  
- 모바일 외국인 등록증 기능
  
<br>

## 📊 기대 효과
- 환율 최적화 → 학기당 약 25만 원 절감 효과  
- 외국인 등록증 기반 금융 접근성 강화  
- 커뮤니티/멘토링으로 문화 적응과 소속감 증대
  
<br>

## 📏 시스템 아키텍처
<p align='center'>
    <img src="https://ifh.cc/g/tABowl.jpg">
</p>

<br>

## 📁 기술 스택
| 영역 | 기술 |
|------|------|
| Android | Kotlin, Compose, MVVM, Clean Architecture, Retrofit, Hilt |
| Backend | Spring Boot, JPA, MySQL, Redis |
| AI | Python, FastAPI |
| Infra | Docker, Jenkins, Prometheus, Loki, Grafana |
| 협업 | Git, Notion, Figma |

<br>

## 🔗 활용 API
- **SSAFY 금융 API**
  - 국내, 외화 계좌정보 및 거래내역 조회
  - 국내, 외화 계좌 이체
  - 환율 조회 및 환전 신청
  - 1원 송금 및 검증
- **외부 API**
  - 한국수출입은행 Open API

 <br>

## 백엔드 링크
- [HeyFY Log](http://114.199.133.118:3000)
- [HeyFY api Docs](https://114.199.133.118/swagger-ui/index.html)
<details>
<summary>HeyFY Log 계정</summary>
<div markdown="1">
id: ssafy<br>
password: ssafy
</div>
</details>

 
## 📝 커밋 메시지 컨벤션

### 🔧 커밋 메시지 형식

```
#{ISSUE_NUMBER}: 변경 요약
```

* 이슈가 없는 작업은 [NO-ISSUE]

> 예시:  
> `#10: 로그인 API 구현`

---

### 📚 ISSUE 생성 방식

-  큰 Task 로 부모 ISSUE 생성
-  부모 ISSUE 에 맞는 Sub Task 생성 (최대한 작게 나누기)

<br>

## 🌿 Git Branch 전략

### 브랜치 종류 및 규칙
| 브랜치 | 용도 |
|--------|------|
| `main` | 배포용 (직접 작업 금지) |
| `develop` | 개발 통합 브랜치 |
| `feature/{이슈번호-설명}` | 기능 개발 |
| `fix/{이슈번호-설명}` | 버그 수정 |
| `hotfix/{이슈번호-설명}` | 긴급 수정 |
| `refactor/{이슈번호-설명}` | 리팩토링 |
| `chore/{이슈번호-설명}` | 환경/설정 |


### Workflow
1. 이슈 생성  
2. 기능 브랜치 생성 (`develop` 기준)  
3. 개발 → 커밋 (`#12 [feat]: 로그인 API 구현`)  
4. PR 생성 → 코드리뷰 후 merge  
5. merge된 브랜치는 삭제  
