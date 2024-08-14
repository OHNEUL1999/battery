# 배터리 | Battery

- [배터리의 단위 | Battery Unit](#배터리의-단위--battery-unit)
- [1차 전지, 2차 전지 | Primary Cell, Secondary Cell](#1차-전지-2차-전지--primary-cell-secondary-cell)
- [리튬이온 전지형태별 종류 | Li-Ion Types](#리튬이온-전지형태별-종류--li-ion-types)
    - [Jelly Roll - Stacking vs Winding](#jelly-roll---stacking-vs-winding)

## 배터리의 단위 | Battery Unit

![Battery Unit](./images/battery/unit.png)

|단위(Unit)|설명(Description)|구성(Structure)|전압(Voltage)[V]|
|---|---|---|---|
|셀(Cell)|배터리의 가장 작은 단위<br>Smallest Unit of a Battery||1.2 ~ 4.2|
|모듈(Module)<br>|여러 셀을 직/병렬 연결한 구조, 배터리 팩의 중간 단계<br>A structure combining multiple cells in series/parallel, an intermediate unit of a battery pack|셀(Cell), 배터리 커넥터(Battery Connectors), 배터리 관리 시스템(BMS), 케이스(Casing)|
|팩(Pack)<br>|모듈의 통합 단위<br>an integral unit assembled from multiple battery modules|배터리 모듈들(Severla Battery Modules), 배터리 커넥터(Battery Connectors), 냉각 시스템(Cooling System), 전기적 인터페이스(Electrical Interface), 케이스(Casing)||
* cell to Pack이라고 모듈을 만들지 않고 바로 팩으로 만들기도 함

## 1차 전지, 2차 전지 | Primary Cell, Secondary Cell

![CELL 종류](./images/battery/cell%20tree.png)

|1차 전지(Primary Cell)|2차 전지(Secondary Cell)|
|---|---|
|방전(discharge)|충방전(charge/discharge)|
|망간(Mn)건전지, 알칼리(Alkali)건전지|리튬이온(Li-Ion), 리튬폴리머(Lithium Polymer), 니켈카드전지(Nickel-cadmium), 니켈수소전지(Nickel-hydrogen) 등|

* 메모리 효과(Memory Effect) : (주로 니켈류) 전지의 용량이 남아있는 상태에서 충전을 하게 되면 남아있던 전지의 용량을 사용하지 못하게 되는 현상 -> 방전 후 충전을 시키면 다시 전부 사용 가능해짐


* 스웰링 현상/배부름 현상(Swelling Phenomenon/Fullness Phenomenon) : (주로 리튬이온류)배터리의 전해액이 산화하며 발생하는 가스로 인해 배터리 내부에 가스가 차는 현상

## 리튬이온 전지형태별 종류 | Li-Ion Types
|구분|특징|
|---|---|
|원통형(Cylindrical Type)<br>![Cylindrical Type](./images/battery/cylineder.png)|- 원통형 스틸 캔 케이스<br>- 크기 작음<br>- 전통적 형태로 규격화된 사이즈
|장점|- 가격 저렴<br>- 대량 생산 용이<br>- 부피당 에너지 밀도 높음|
|단점|- 전기차 배터리 시스템 구축 시 고비용<br>- 낮은 에너지 밀도<br>- 짧은 수명|
|==========|==========|
|각형(Square Type)<br>![Square Type](./images/battery/square.png)|- 알루미늄 캔 케이스<br>- 여러개 쌓기 가능|
|장점|- 외부 충격에 강함<br>|
|단점|- 내부 공간 활용 측면에서 불리<br>- 제조 공정이 상대적으로 복잡함<br>- 형태변경 어려움<br>- 무거움|
|==========|==========|
|파우치형(Pouch Type)<br>![Pouch Type](./images/battery/pouch.png)|- 부드러운 필름으로 포장<br>- 내부 공간 꽉 참<br>- 얇음
|장점|- 공간 효율 좋아 에너지 밀도 높음<br>- 다양한 배터리 디자인 가능|
|단점|- 다른 형태에 비해 케이스가 단단하지 않아 모듈이나 팩 제작시 커버 필요<br>- 낮은 생산성<br>- 내구성 약함|

### Jelly Roll - Stacking vs Winding
![Winding & Stacking](./images/battery/wind&stack.png)

- 원형 : Jelly Roll 그대로
- 각형 & 파우치형 : Jelly Roll 압착 후 casing 하거나 stack

=> Winding방식 후 압착한 경우 양 옆에 열이 나서 C-rate가 중요함!
<br>압착하지 않은 경우(주로 원통형) 저항이 일정함

* 리튬의 전착 (Electroplating) : 음극의 대면이 양극보다 큼! 아닐 경우 충전시 양극에서 빠져나운 리튬이 음극의 모서리에서 석출됨
