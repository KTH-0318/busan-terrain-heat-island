[README.md](https://github.com/user-attachments/files/32555072/README.md)
# 안녕하세요, 김태형입니다 

### 스포츠 데이터 분석가를 지향하는, 스마트시티 문제를 공간 분석으로 풀어온 데이터 분석가

- **스포츠 데이터로 결과를 만들어봤습니다** — KBO 시즌 순위(6/10팀 적중, 우승·준우승 예측)와 NBA 플레이오프(우승팀·파이널 스코어 4-3 적중)를 실제 결과로 검증했습니다
- **스마트시티 문제는 문제 설계부터 합니다** — 경사 반영 보행 네트워크(서울), 다기준 의사결정 파이프라인(대전), 위성 데이터로 지형 효과를 실증한 열섬 진단(부산)까지, 도시마다 다른 접근을 직접 설계했습니다
- **분석에서 끝내지 않습니다** — 크롤링으로 데이터를 직접 수집하고, 라즈베리파이 + YOLO 시스템을 실제 열람실 72석에 배포·시연한 경험이 있습니다

한남대학교 빅데이터응용학과 (2023.03 ~ 2027.02)

**전체 포트폴리오 (STAR 상세 페이지) → [Notion](https://zany-meeting-aba.notion.site/e6783f9aaedb8289bbbb016f91607fa9)**

---

## Sports Analytics 

| 프로젝트 | 핵심 | 검증된 결과 |
| --- | --- | --- |
| [KBO 승부 예측](https://github.com/KTH-0318/kbo_win_prediction)  | 크롤링 → 파생변수 설계 → 포아송 회귀 | 순위 6/10 적중 · 우승/준우승 예측 · ρ≈0.87 |
| [NBA 플레이오프 예측](https://github.com/KTH-0318/nba_win_prediction) | XGBoost 득점 예측 + 몬테카를로 1,000회 | 우승팀(OKC)·파이널 스코어 4-3까지 적중 |

## Smart City × Spatial Analysis 

| 프로젝트 | 문제 유형 | 접근 |
| --- | --- | --- |
| [서울 대중교통 취약지역](https://github.com/KTH-0318/Seoul_transit_accessibility) | 접근성 진단 | Tobler 경사 네트워크(21만 노드) + Dijkstra + 2SFCA + 사분면 분석 |
| [대전 트램 정거장 타당성](https://github.com/KTH-0318/daejeon_tram_station_analysis) | 다기준 의사결정 | 네트워크 중심성 → KMeans → 시나리오 → TOPSIS → GIS 등급화 |
| [부산 산지 열섬 진단](https://github.com/KTH-0318/busan-terrain-heat-island) | 원인 진단 (기후·지형) | 위성 LST 64,915격자 → LISA 열섬핵 → 위계적 회귀(지형 추가 시 산지 ΔR² 평지의 2.6배) → 원인 유형화 |

## System Building

| 프로젝트 | 핵심 |
| --- | --- |
| [실시간 열람실 모니터링](https://github.com/KTH-0318/reading_room_monitoring)  | 라즈베리파이 + YOLOv8n + 환경센서 → MySQL → 웹 대시보드. 얼굴 대신 물건 탐지로 프라이버시 배려, 실제 72석 배포 |

<details>
<summary><b> 그 외 프로젝트 (8) — 펼쳐보기</b></summary>

<br>

| 프로젝트 | 한 줄 요약 |
| --- | --- |
| [천안 쿨링포그 입지](https://github.com/KTH-0318/Cheonan_coolingfog-priority) | 정답 없는 입지 문제 — 프록시 도시(대전) 역추적 → 행정동 → 150m 헥스 2단계 줌인 |
| [영천시 교통·복지 사각지대](https://github.com/KTH-0318/Yeongcheon_blindspot_analysis) | 복합 고립지수 설계 + 분위 4등급화 → 정책 우선순위 |
| [날씨 기반 119 신고 예측](https://github.com/KTH-0318/weather-119-call-prediction) | 3종 앙상블 + TimeSeriesSplit + 자기회귀 순차 예측 (RMSE 5.7) |
| [대전 지하철 수요 예측](https://github.com/KTH-0318/Daejeon_subway_demand_forecast) | 스마트카드 + 400m 버퍼 공간변수 결합 → 역별·시간대별 예측 |
| [보험료 기반 Risk 추정](https://github.com/KTH-0318/insurance_risk_pricing) | 순보험료 → 요율요소 → 상대도·Off-Balancing → 계산기 구현 |
| [딥페이크 AI 탐지](https://github.com/KTH-0318/deepfake_dectection) | video 단위 분할(누수 방지) + EfficientNet 앙상블 + Grad-CAM |
| [1인 가구 배달앱 소비 분석](https://github.com/KTH-0318/delivery_app_regression) | 설문 직접 설계(61명) + 회귀 가설검정 + 모형 진단 |
| [손상 보도블럭 탐지](https://github.com/KTH-0318/sidewalk_damage_dectection) | YOLO11n · 1,018장 직접 라벨링 · 보행 보조 활용안 |

</details>

---

##  SKILL

> 각 기술의 활용도를 최대 3개의 ⭐로 표시 (상/중/하)

| 분류 | 스택 |
| --- | --- |
| 언어 | Python ⭐⭐⭐ · R ⭐⭐⭐ · SQL ⭐⭐ |
| 데이터 수집 | Selenium · BeautifulSoup |
| 분석·모델링 | scikit-learn · XGBoost · LightGBM · CatBoost · PyTorch · Ultralytics YOLO · OpenCV · statsmodels · K-Means/PCA |
| 공간 분석 | QGIS ⭐⭐⭐ · GeoPandas · Folium · Google Earth Engine · PySAL |
| 환경·도구 | VS Code · R Studio · Git/GitHub · MySQL · Excel · Notion · MobaXTerm |

##  Awards & Certification

-  2025년도 오픈데이터 자료 활용 KBO 빅데이터 콘테스트 — **한남대학교 스마트융합대학장상** (2025.11)
-  지역사회 문제해결형 빅데이터/AI 활용 공모전 — **한남대학교 총장상** (2025.02)
-  소프트웨어 인재육성 캠프 — **동상** (2024.08)
  
-  ADsP 데이터분석 준전문가 (2024.09)

##  Contact

- Email: q288712a@gmail.com
- Portfolio: https://zany-meeting-aba.notion.site/e6783f9aaedb8289bbbb016f91607fa9
