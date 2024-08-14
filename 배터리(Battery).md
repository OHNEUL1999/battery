# 배터리 | Battery

- [배터리의 단위 | Battery Unit](#배터리의-단위--battery-unit)
- [1차 전지, 2차 전지 | Primary Cell, Secondary Cell](#1차-전지-2차-전지--primary-cell-secondary-cell)

## 배터리의 단위 | Battery Unit

![Battery Unit](./images/battery/unit.png)

|단위(Unit)|설명(Description)|구성(Structure)|전압(Voltage)[V]|
|---|---|---|---|
|셀(Cell)|배터리의 가장 작은 단위<br>Smallest Unit of a Battery||1.2 ~ 4.2|
|모듈(Module)<br>|여러 셀을 직/병렬 연결한 구조, 배터리 팩의 중간 단계<br>A structure combining multiple cells in series/parallel, an intermediate unit of a battery pack|셀(Cell), 배터리 커넥터(Battery Connectors), 배터리 관리 시스템(BMS), 케이스(Casing)|
|팩(Pack)<br>|모듈의 통합 단위<br>an integral unit assembled from multiple battery modules|배터리 모듈들(Severla Battery Modules), 배터리 커넥터(Battery Connectors), 냉각 시스템(Cooling System), 전기적 인터페이스(Electrical Interface), 케이스(Casing)||
* cell to Pack이라고 모듈을 만들지 않고 바로 팩으로 만들기도 함

## 1차 전지, 2차 전지 | Primary Cell, Secondary Cell

|1차 전지(Primary Cell)|2차 전지(Secondary Cell)|
|---|---|
|방전(discharge)|충방전(charge/discharge)|
|망간(Mn)건전지, 알칼리(Alkali)건전지|리튬이온(Li-Ion), 리튬폴리머(Lithium Polymer), 니켈카드전지(Nickel-cadmium), 니켈수소전지(Nickel-hydrogen) 등|

* 메모리 효과(Memory Effect) : (주로 니켈류) 전지의 용량이 남아있는 상태에서 충전을 하게 되면 남아있던 전지의 용량을 사용하지 못하게 되는 현상 -> 방전 후 충전을 시키면 다시 전부 사용 가능해짐


* 스웰링 현상/배부름 현상(Swelling Phenomenon/Fullness Phenomenon) : (주로 리튬이온류)배터리의 전해액이 산화하며 발생하는 가스로 인해 배터리 내부에 가스가 차는 현상
