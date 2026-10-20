<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Data%20Engineer&fontSize=56&fontAlignY=38&desc=Chemistry%20%C3%97%20Data%20%C3%97%20Security&descAlignY=58" />
</p>

<h3 align="center">안녕하세요, 데이터 엔지니어를 준비하고 있는 황도희입니다 👋</h3>
<p align="center">데이터가 빠지거나 중복되지 않고, 다시 돌려도 같은 결과가 나오는 파이프라인을 만드는 데 관심이 많습니다.</p>

<p align="center">
  <a href="mailto:s2nardh@gmail.com"><img src="https://img.shields.io/badge/Gmail-s2nardh@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
</p>

<br>

## 🙋‍♀️ About Me

- 이화여자대학교 화학·나노과학과 졸업 (소프트웨어 융합연계전공 복수전공)
- SKALA 4기 AI·데이터 과정 수강 중 (2026.07 ~ 2026.12)
- 한국인터넷진흥원(KISA) AI 보안관제 전문인력 양성과정 8기 수료

<br>

## 🛠️ Tech Stack

**Language**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**Data / Infra**  
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka%20(Redpanda)-231F20?style=flat-square&logo=apachekafka&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white)

**Backend**  
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)

**ML / Analysis**  
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)

<br>

## 📌 Projects

### [[kpi-sentinel](https://github.com/ahrdyrxkddhfl/kpi-sentinel)] 실시간 KPI 이상 감지 파이프라인
`Python` `Redpanda(Kafka)` `PostgreSQL` `DuckDB` `Docker Compose`
- 요일·시간대별 기준값과 EWMA로 계절성을 반영해 단순 임계값 방식보다 오탐 77% 감소 (장애 미탐 0건 유지)
- 컨슈머를 처리 도중 강제 종료해도 유실·중복 없이 적재되는지 커밋 전략별로 실험
- 배치와 스트림이 같은 집계 코드를 쓰도록 만들어 두 경로의 결과가 일치하는지 확인
- 알람이 울린 근거를 지표 단위로 남기고, LLM으로 운용자용 장애 리포트 작성

### [[mfds-drug-pipeline](https://github.com/ahrdyrxkddhfl/mfds-drug-pipeline)] 식약처 의약품 공공데이터 수집·정제 파이프라인
`Python` `PostgreSQL` `Docker Compose` `pytest`
- 원본 저장 → 정규화 → 검증 단계를 나눠, 정제 규칙을 고칠 때 API를 다시 호출하지 않고 변환만 재실행
- 허가정보 42,980건을 제품 42,885개로 정리하고, upsert로 여러 번 실행해도 결과가 같게 구성
- 품질 검사 규칙 8종을 매 배치마다 기록해 성분명 파싱 버그를 찾아 불일치 244건 → 67건으로 감소
- 실데이터에서 발견한 사례 위주로 단위 테스트 48개 작성

### [[claim-trace](https://github.com/ahrdyrxkddhfl/claim-trace)] AI 보험금 심사 근거 추적 시스템
`Java 21` `Spring Boot` `JPA` `PostgreSQL`
- AI 권고와 심사자 판정을 따로 저장하고, 채택·기각한 근거를 항목별로 남기도록 데이터 모델 설계 (엔터티 16개, API 36개)
- 설계 때 정한 불변조건 13개를 코드로 강제하고 테스트 102개로 검증
- 설계부터 백엔드 구현까지 혼자 진행

### [[taxi](https://github.com/SKALA-python/taxi)] NYC 로보택시 배차 전략 (팀 6인)
`Python` `pandas` `scikit-learn`
- NYC 옐로우택시 운행 데이터 388만 건으로 수요·건당 수익·효율 예측 모델을 만들어 배차 우선순위 제안
- 모델 파트를 맡아 모델별 방향과 공통 산출물 규격을 정했고, 팀원들이 나눠 만든 코드가 거의 수정 없이 한 번에 통합 실행됨
- 효율(RPM) 모델 개발과 세 모델 통합 담당

### [[SKALA_CNN-Optimization](https://github.com/ahrdyrxkddhfl/SKALA_CNN-Optimization)] 웨이퍼맵 불량 분류 CNN 개선 (팀 2인)
`Python` `PyTorch`
- 파라미터의 97.6%가 FC 한 층에 몰린 구조 때문에 과적합이 생긴 것으로 진단
- Conv 4블록 + BatchNorm + GAP로 구조를 바꿔 Test Macro-F1 0.755 → 0.881, 파라미터 71% 감소
- 두 사람이 각자 진행한 실험 중 최종안으로 채택

<br>

## 🧰 Other Projects

**Security**
- [[binary-analyzer-mcp](https://github.com/ahrdyrxkddhfl/binary-analyzer-mcp)] ELF 바이너리의 위험 함수와 보호기법을 분석해 익스플로잇 난이도를 알려주는 MCP 서버
- [[evidence-trace](https://github.com/ahrdyrxkddhfl/evidence-trace)] 망분리 환경용 로컬 포렌식 조사 보조 AI, 답변마다 원본 증거까지 추적
- [[ForensicFileAnalyzer](https://github.com/ahrdyrxkddhfl/ForensicFileAnalyzer)] 증거 파일의 해시·실제 형식·시간 정보를 기록하고 확장자 위장을 탐지하는 CLI
- [[CAN-ADS](https://github.com/ahrdyrxkddhfl/CAN-ADS)] 정상 주행 데이터만으로 학습한 차량 CAN 통신 침입 탐지

**Manufacturing**
- [[wafer-lot-hold](https://github.com/ahrdyrxkddhfl/wafer-lot-hold)] AI 검사 결과로 불량 Lot을 자동 정지하고, 해제·재검사·폐기는 사람이 결정하는 MES 기능 구현 (FastAPI, PostgreSQL)

**Tools**
- [[vibecheck](https://github.com/ahrdyrxkddhfl/vibecheck)] AI로 짠 코드를 내가 설명할 수 있는지 확인하는 면접 연습 도구 ([PyPI 배포](https://pypi.org/project/vibecheck-whyd/))
- [[crumb-tracker](https://github.com/ahrdyrxkddhfl/crumb-tracker)] 바이브코딩 작업 기록을 작업일지와 트러블슈팅 목록으로 정리해주는 로컬 도구

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=footer" />
</p>
