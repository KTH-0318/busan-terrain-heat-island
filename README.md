# 산지도시 부산의 야간 열섬 진단

부산 전역 100m 격자 64,915셀의 위성·지형·건물 데이터로, 평지 도시 기준의 열섬 모델이 산지 도시에서는 설명력이 떨어진다는 것을 실증한 공간 분석 프로젝트. 지형 변수 추가 시 산지의 설명력 증가분(ΔR² +0.107)이 평지의 2.6배 · 열섬핵 5개 원인 유형 분류 · 행정동 206개 대응 우선순위 도출. 2026 부산광역시 빅데이터 활용 경진대회(DX CHALLENGE) 트랙1 출품작.

📌 프로젝트 상세 → Notion 포트폴리오

분석 흐름 및 파일 구성
단계	파일	내용
1. 위성 LST	notebooks/[파트1 파일명]	ECOSTRESS·Landsat 수집, 품질 필터, 격자 집계
2. 지형 변수	notebooks/[파트2 파일명]	DEM → 경사·TPI·남서향·지형 SVF
3. 신뢰도 검증	notebooks/[파트3 파일명]	AWS 지상 관측과 위성 LST 매칭 검증 (148쌍)
4. 건물·사회 변수	notebooks/[파트4 파일명]	건폐율·용적밀도·바람길·NDVI·사회지표
5. 통합 분석	notebooks/[파트5 파일명]	LISA 열섬핵 → 위계적 회귀 → 공간 교차검증 → 유형화 → 우선순위
검증	scripts/	시각화 빌더 3종 · 수치 대조 및 독립 재계산 검증 6종
결과	data_sample/	파생 결과 CSV 13종 (열 설명 사전 포함)
문서	docs/	보고서 · 데이터 시각화 PDF

👉 결과만 보려면 파트5 노트북 하나만 열어도 됩니다.

데이터

NASA LP DAAC(ECOSTRESS) · USGS(Landsat) · ESA(Sentinel-2) · 국토지리정보원 · 기상청 · 환경부 · 국가공간정보포털 · 통계청 SGIS

원자료(약 3.5GB)는 용량과 배포 조건 때문에 포함하지 않았습니다. 위 출처에서 동일 데이터를 받을 수 있습니다.

기술 스택

Python geopandas rasterio h3 statsmodels esda mgwr PyTorch Google Earth Engine
