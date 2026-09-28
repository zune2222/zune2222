# 박준이 · Software Engineer

**AI·SW마에스트로 17기 연수생** · Backend · AI Systems · Web & Mobile

웹·모바일 화면부터 백엔드 API, 데이터 파이프라인, AI 모델 서빙과 운영까지 연결합니다.
현재 부산대학교 AI융합교육원에서 AI역량지원시스템을 개발하고, AI·SW마에스트로 팀 MOSS에서 음성 기반 현장 기록 서비스 **김경리**를 만들고 있습니다.

[Email](mailto:zun_e@kakao.com) · [Blog](https://zune2222.github.io) · [LinkedIn](https://www.linkedin.com/in/%EC%A4%80%EC%9D%B4-%EB%B0%95-3304b4330/)

## 현재 하는 일

### AI·SW마에스트로 17기 · Team MOSS

2026.05 — 현재 · **김경리: 음성 기반 현장 공수 기록 서비스**

- Android 음성 인식·TTS와 React WebView를 연결해 말하기, 되읽기, 수정·저장 확인 흐름을 구현했습니다.
- 취소 후 늦게 도착한 응답을 폐기하고, TTS 종료 후 마이크 전환과 인식 실패 시 텍스트 입력을 처리했습니다.
- 회원 탈퇴 시 단말의 푸시 식별자와 서버의 비활성 토큰을 정리하는 흐름을 구현했습니다.

`Kotlin` `React` `TypeScript` `Spring Boot` · 팀 프로젝트 개발 중, 음성 흐름 구현·모의 테스트 및 빌드 검증

### 부산대학교 AI융합교육원 · 개발 조교

2026.03 — 현재 · **AI역량지원시스템·Career Agent**

- 학생 정보를 외부 LLM API에 보내지 않는 **vLLM 로컬 서빙 환경**과 채용공고 수집·분석 흐름을 구성했습니다.
- 모델 출력 형식과 실제 학생·공고 데이터의 유효성을 나누어 검증하고, 생성 실패 시 규칙 기반 계획기로 전환하는 폴백을 구현했습니다.
- 전공트랙 신청·심사 API의 기간·전공·과목·소유권 검증과 관리자 조회 기능을 개발했습니다.

`Spring Boot` `Python` `vLLM` `Next.js` `Docker`

## 주요 프로젝트

### [TriPick](https://github.com/PNUKoZune/tripick) · 취향 사진 기반 AI 여행 플래너

부산대학교 졸업과제 팀 프로젝트 · [서비스](https://tripick.place) · [코드](https://github.com/PNUKoZune/tripick)

- 취향 태그·목적지 질의에서 **pgvector 검색 → CRAG 후보 평가 → LLM 일정 생성**으로 이어지는 서버 파이프라인을 구현했습니다.
- 영업시간·활동 시간·이동 ETA를 저장 전에 검증하고, 조건 위반 시 일정 저장을 차단하도록 변경했습니다.
- AI 일정안이 실패하면 결정론적 일정안으로 다시 생성하고, 대체안도 유효하지 않으면 기존 일정을 보존합니다.

`TypeScript` `NestJS` `PostgreSQL / pgvector` `RAG / CRAG`

### imarichman · 암호자산 퀀트 자동매매·운영 시스템

개인 프로젝트 · 소스 비공개

- Python·Freqtrade로 시장 데이터 수집, 신호 계산, 리스크 검증, 주문 실행을 연결했습니다.
- 필요한 검증 데이터가 없는 진입 후보를 차단하고, 판단 조건과 차단 이유를 JSONL로 기록합니다.
- 백테스트와 실제 거래 기록의 차이를 대조하는 도구, 컨테이너·API·주문 실패·데이터 갱신 상태를 확인하는 운영 도구를 구현했습니다.

`Python` `Freqtrade` `pandas` `SQLite` `Docker` `Next.js`

### PNU Blace · 도서관 데이터 분석·실시간 좌석 소통

1인 개발·운영 · **현재 운영 종료** · 소스 비공개

- 과거 운영 기간 누적 방문 **7,203명**, 페이지뷰 **56,271회**를 기록했습니다.
- Next.js·NestJS 모노레포에서 서버 조회와 캐시 전달을 공통화하고, 독립적인 통계 조회를 병렬화했습니다.
- 실시간 연결의 수명과 화면 상태를 분리하고, 좌석 점유 이력에 조건부 생존분석을 적용해 공석 확률과 잔여시간 범위를 계산했습니다.

`Next.js` `NestJS` `PostgreSQL` `Redis` `Socket.IO`

### [PNU IBE](https://github.com/zune2222/PNU-IBE) · 학생회 물품 대여·행사 운영

웹사이트 및 관련 서버 개발 · [서비스](https://pnu-ibe.web.app/) · [웹 코드](https://github.com/zune2222/PNU-IBE)

- 담당자가 처리하던 물품 대여·반납을 학생이 직접 진행하는 웹 흐름으로 전환했습니다.
- 학생증 OCR, 대여·반납 사진 증빙, 미수령 처리와 보관함 변경 이력 등 관리자 기능을 구현했습니다.
- 별도 Spring Boot 서버에서 e스포츠 참가·팀·결과·포인트 승부예측·랭킹 API를 개발했습니다.

`Next.js` `Firebase` `Tesseract.js` `Spring Boot` `PostgreSQL`

## 출시한 모바일 앱

| 앱 | 역할과 구현 |
| --- | --- |
| **K-Lingo** · 한국어 학습 | 에버스톤 현장실습에서 기획·디자인·개발과 iOS·Android 출시에 참여. 시즌 리더보드의 프로필 묶음 조회, 시즌별 캐시와 초기화 예외 처리를 구현했습니다. [App Store](https://apps.apple.com/kr/app/k-lingo/id6740884844) · [Google Play](https://play.google.com/store/apps/details?id=com.evst.klingo) |
| **Katter** · 예약 편지·커플 SNS | 1인 기획·디자인·개발로 iOS·Android 출시. React Native·Expo·Firebase를 사용해 예약 편지, 이미지 캐시, 화면별 제스처와 iOS 로컬 알림 재스케줄링을 구현했습니다. [Google Play](https://play.google.com/store/apps/details?id=com.zuraft.katter) |

<details>
<summary><strong>다른 프로젝트와 초기 작업 29개 보기</strong></summary>

| 프로젝트 | 내용 |
| --- | --- |
| 오늘모했냥 → 우리모하냥 | 팀 커플 앱에서 출발해 개인 저장소에서 후속 개발. 기록·사진 복구의 부분 실패 처리, Android·iOS 비동기 브리지, 채팅·방문 기록 |
| Glue | 언어 교환 모임 매칭 팀 프로젝트. React Native·Spring Boot 환경에서 S3 리소스 경로와 인증 구조 개선 제안 |
| GongByeol · 공별 | React Native·Firebase 기반 실시간 채팅·피드·미니게임 SNS |
| AliStory · AlisTouch | 외국인 근로자 법률 상담·커뮤니티 팀 프로젝트의 Next.js 프론트엔드 |
| BMS Control System | Next.js·Spring Boot·Python과 MQTT·STOMP를 연결한 배터리 계측·제어 대시보드 |
| Home Assistant | Raspberry Pi·Zigbee·MQTT 기반 조명·커튼·에어컨 로컬 자동화 |
| Habaragi Survival | Phaser 게임, Next.js·Firebase와 React Native WebView를 연결한 미니게임 |
| 이거무라 | 개인·그룹 식당 추천 팀 프로젝트. 로그인·회원가입과 인프라·배포 담당 |
| eatPnu | 부산대학교 주변 맛집 추천 웹서비스 |
| zun2log | 군 복무 중 시작한 Next.js·MDX 기술 블로그와 GitHub Actions 배포 |
| 2MonthosOfLetters · 2MOL | 입대 전 작성한 인터넷 편지를 전달하는 웹서비스 |
| 1to50 | React·Firebase로 만든 숫자 순서 누르기 게임 |
| potNative | React Native·Firebase 앱과 Arduino 센서를 연동한 식물 관리 수업 프로젝트 |
| XROS | ABlock에서 개발한 React Native·Expo 지도 기반 앱. 마커 군집화와 캐시 정책 적용 |
| EchoPang | 2024 BEST Challenge ESG 해커톤 팀 프로젝트. Next.js 대시보드·보상·상품 교환 화면과 ethers 연동 |
| 생갓하고 살자 | 2022 부산 ICT 해카톤 팀 프로젝트. React Native·Expo 생활 관리 앱 프론트엔드 |
| TaxiCab | 2021 부산 ICT 해카톤 AI 택시 매칭 팀 프로젝트 |
| LivinBusan | 성향 입력·부산 지역 추천·채팅 화면을 구성한 팀 웹 프로토타입 |
| Questura | 그룹·채팅·성향 입력을 구성한 해커톤 모바일 프로토타입 |
| FlavGuide | 식단·재료·레시피 안내를 위한 React Native·Expo 모바일 프로토타입 |
| CapturePlanner | 이미지 업로드·AI 대화·캘린더를 연결하는 모바일 UI 프로토타입 |
| 공실 상가 지도 | 네이버 지도 기반 공실 탐색·조건 필터·상권 분석 웹 프로토타입 |
| 외로운 솔로 | 결정론적 점수·Hungarian assignment와 WebSocket, 로컬 Qwen을 사용하는 매칭 실험 |
| SUDO | Next.js·NestJS·Prisma·PostgreSQL 기반 루틴·알림 초기 프로토타입 |
| SomaBiseo | AI·SW마에스트로 공지·멘토링 일정 탐색과 추천을 돕는 비공식 팀 프로젝트 |
| BNK 로컬 챌린지 | 관심 카테고리·지역 미션·지도·참여 흐름을 구성한 해커톤 모바일 웹 |
| AIrena | 강화학습 게임 교육 플랫폼의 초기 웹 프로토타입 |
| Our Next Page | 스마트폰과 메인 스크린을 연결하는 인터랙티브 웹 초기 기획·프로젝트 구조 |
| xv6 Copy-on-Write | 페이지 공유·참조 수 관리, 쓰기 예외 시 복사와 메모리 반환을 구현한 운영체제 과제 |

</details>

## 기술

| 영역 | 사용 기술 |
| --- | --- |
| 언어 | Python, TypeScript, JavaScript, Java, SQL, C, C++ |
| 백엔드 | Spring Boot, NestJS, FastAPI, Socket.IO, WebSocket, BullMQ |
| AI·데이터 처리 | vLLM, RAG·CRAG, 구조화 출력, pandas, Polars |
| 데이터 저장 | PostgreSQL, pgvector, Redis, MySQL, Firebase, DuckDB, SQLite |
| 웹·모바일 | React, Next.js, React Native, Expo, Kotlin, SwiftUI, TanStack Query |
| 배포·품질·운영 | Docker, AWS, GitHub Actions, Playwright, Vitest, JUnit, Pytest, Sentry |

## 경력·학력

| 기간 | 경험 |
| --- | --- |
| **2026.05 — 현재** | **AI·SW마에스트로 17기 연수생** · 팀 MOSS, 김경리 개발 |
| **2026.03 — 현재** | **부산대학교 AI융합교육원 개발 조교** · AI역량지원시스템·Career Agent |
| 2024.12 — 2025.07 | **에버스톤(EVST)** · K-Lingo 개발·출시, 부산대학교 단기·장기 현장실습 |
| 2021.12 — 2022.07 | **ABlock · Frontend Engineer** · XROS 모바일 앱 개발 |
| 2021.03 — 2021.05 | **ZUDA · Frontend Engineer** · 웹 퍼블리싱·jQuery·Firebase 실시간 채팅 |
| 2021.03 — 2027.02 예정 | **부산대학교 정보컴퓨터공학부** · SW특기자 전형 입학, 학사 졸업 예정 |

육군 네트워크운용·정비병 복무: 2022.09 — 2024.03

## 수상 · 16개

| 연도 | 수상 |
| --- | --- |
| 2025 | **BNK 디지털 혁신 챌린지 해커톤 최우수상** · BNK금융그룹 |
| 2024 | [블록체인 경진대회 BEST Challenge ESG 해커톤 최우수상 · 한국인터넷진흥원장상](https://www.notion.so/f16d2073461f42d8bca169d44e00e431) |
| 2024 | [제1회 코드코리아 2024 금정구 해커톤 대상](https://www.notion.so/81e2e1117a3642fb949e185aa994e312) |
| 2023 | [제1회 나의 꿈 발표 대회 장려상](https://www.notion.so/9148cef637f74595b30a51265b40b731) |
| 2022 | [제7회 부산 ICT 융합 해카톤 일반부 우수상](https://www.notion.so/e1685e9e81694294b9e9b305350147b4) |
| 2021 | [제6회 부산 ICT 융합 해카톤 일반부 대상](https://www.notion.so/d7dcb89715844b0dafe26c2bcf139626) |
| 2020 | [Smarteen App+ Challenge 2020 미래산업 부문 우수상](https://www.notion.so/2682e7e61ae44cccb3429e90405a27e0) |
| 2020 | [제5회 부산 ICT 융합 해카톤 대회 열정상](https://www.notion.so/489915c0986b4527a38d68c50340704c) |
| 2020 | [AI 기반 프로젝트학습 경진대회(더 나은 부산 만들기) 산학협력단장상](https://www.notion.so/51a48cb492a946a78103cf8ed17fd833) |
| 2020 | [인공지능 Hackademy 최우수상 · 부산대학교 소프트웨어교육센터장상](https://www.notion.so/611675cf2abd41e29456b43eb5217243) |
| 2019 | [동래고등학교 군봉 해카톤대회 우수상](https://www.notion.so/32bc5041310e4227ac6d58c575ae0a90) |
| 2019 | [디지털 사회혁신(DSI) 아이디어 공모대회 최우수상](https://www.notion.so/dd31538142a647ae86ab8f7992e322e5) |
| 2019 | [제1회 부경 크리에이티브 메이커톤 경진대회 최우수상](https://www.notion.so/5becf55b7a2642cb902e37d66e912673) |
| 2019 | [제3회 부산 SW교육 중등학생 해카톤 대회 장려상](https://www.notion.so/63cd8d895bf64e6d8b0e05b18b4a1c74) |
| 2019 | [제2회 한국 메이커 & 코딩 경진대회 메이커 부문 대상 · 중소벤처기업부장관상](https://www.notion.so/802b807aa47b4dfe9d7a8e316ed9f431) |
| 2019 | [우송대학교 제1회 전국고교SW동아리 경진대회 장려상](https://www.notion.so/3e9a9cc7ae9546e3b9e38943d877206e) |

<details>
<summary>GitAnimals</summary>

<a href="https://www.gitanimals.org/en_US?utm_medium=image&utm_source=zune2222&utm_content=farm">
  <img src="https://render.gitanimals.org/farms/zune2222" width="100%" alt="zune2222의 GitAnimals 농장" />
</a>

</details>

<sub>Updated 2026.09.28</sub>
