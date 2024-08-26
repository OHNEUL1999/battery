# 배터리 관리 시스템 | Battery Management System, BMS

- [개요 | Outline](#개요--outline)
    - [정의 | Definition](#정의--definition)
    - [기능 | Function - HW](#기능--function---hw)
    - [기능 | Function - SW](#기능--function---sw)
    - [필요성 | Neccessafy](#필요성--necessary)
    - [연구 동향 | Research Trends](#연구-동향--research-trends)

## 개요 | Outline
### 정의 | Definition
배터리의 전압, 온도, 전류 등을 센서 기반으로 측정하여 배터리가 최적의 성능을 낼 수 있도록 제어하는 시스템<br>A system that measures battery voltage, temperature, and current using sensors to control the battery for optimal performance.

- 전기자동차의 BMS 기능 : 배터리 상태 추정(Sox), 충전 제어, 고장 진단, 열 관리 등<br>BMS functions for electric vehicles: Battery state estimation (SoX), charging control, fault diagnosis, thermal management, etc.

### 기능 | Function - HW
전자제어장치의 한 종류로 디지털 회로와 아날로그 회로 조합으로 구성됨<br>A type of electronic control unit consisting of a combination of digital and analog circuits.

`BMS HW`란 배터리를 관리 및 제어하는 물리적 부품을 의미한다.<br>`BMS HW` refers to the physical components that manage and control the battery.

### 기능 | Function - SW
배터리의 전압/전류/온도 등 정보를 측정 및 수집하고, 정보를 기반으로 상태 지표를 추정한다.<br>Measures and collects information on battery voltage, current, and temperature, and estimates state indicators based on this information.

`상태 지표(SOx)`는 SOC, SOH, SOP등이 있다.<br>`State indicators (SoX)` include SOC, SOH, SOP, etc.

### 필요성 | Necessary
- 전기자동차 시장 확대에 따른 리튬이온 배터리 수요 증가<br>Increasing demand for lithium-ion batteries due to the expansion of the electric vehicle market.
    - 2030까지 전기자동차용 배터리는 1,033GWh로 성장할 것으로 전망<br>The battery market for electric vehicles is expected to grow to 1,033 GWh by 2030.
    - 2036에는 신차 판매 점유율에서 전기자동차가 내연기관차 앞설 것으로 전망<br>By 2036, electric vehicles are expected to surpass internal combustion engine vehicles in new car sales share.
- 다양한 친환경 에너지 정책 시행으로 EV(Electric Vehicle) 및 배터리 시장의 지속적인 확대<br>Continuous expansion of the EV and battery markets due to various eco-friendly energy policies.
    - 재생에너지 3020, 탄소 중립(Net-zero) 등<br>Policies include Renewable Energy 3020 and Net-zero carbon initiatives.
- 전기자동차 보급을 확대하기 위해 보조금 지원 및 충전 인프라 구축 예산 증진<br>Expansion of subsidies and charging infrastructure budgets to promote electric vehicle adoption.
    - 보조금 정책 2022 종료 예정에서 2025로 연장 (4조 5천억 투입)<br>Subsidy policy extended from 2022 to 2025 with 4.5 trillion won allocated.
- 리튬이온 배터리 화재 사고로 인한 배터리 안전성 위협<br>Safety concerns due to lithium-ion battery fires.
    - 지속적인 화재 사고 발생 (SOC 90↑ 화재위험)<br>Ongoing fire incidents (Fire risk at SOC 90% and above).
    - BMS 성능 고도화 요구됨<br>Need for advanced BMS performance.
    - 전기자동차 화재의 원인 : 배터리 결함, BMS 결험 지목됨<br>Causes of electric vehicle fires: Battery defects and BMS defects identified.
- 리튬이온 배터리 시스템의 대용량/고출력 적용 가속화<br>Acceleration of large-capacity/high-power applications of lithium-ion battery systems.
    - 배터리 시스템은 다수의 셀이 직/병렬 조합으로 구성되어 있어 `셀 단위 모니터링의 한계`있음<br>Battery systems are composed of multiple cells in series/parallel combinations, resulting in limitations in cell-level monitoring.


### 연구 동향 | Research Trends
- 저렴한 가격으로 LFP 배터리 수요 및 시장 증가하므로 관련 연구 개발 필요함<br>Growing demand and market for LFP batteries at lower costs necessitate related research and development.
- LFP 배터리 특성에 따른 부정확한 OCV 발생함 → 일정 SOC 영역의 평탄구간 존재함<br>Inaccurate OCV (Open Circuit Voltage) due to LFP battery characteristics, leading to flat regions in certain SOC ranges.
- SOC 추정 위한 다양한 기법 연구<br>Research on various techniques for SOC estimation.
    - 충전 프로파일별 전압 데이터 입력에 따른 SOC 추정<br>SOC estimation based on voltage data inputs from different charging profiles.
    - 건전성 지표 활용한 낮은 영역의 SOC 추정<br>SOC estimation in lower ranges using health indicators.
