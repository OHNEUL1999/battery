# 회로 | Circuit

- [회로 | Circuit](#회로--circuit)
  - [용어 | Terminology](#용어--terminology)
  - [소자 | Element](#소자--element)
  - [전원 | Source](#전원--source)
  - [전압 | Voltage](#전압--voltage)
    - [옴의 법칙 | Ohm's Law](#옴의-법칙--ohms-law)
  - [회로 해석 | Circuit Analysis](#회로-해석--circuit-analysis)
    - [회로해석을 위한 기본단위 | Fundamental Units in Circuit Analysis and Design](#회로해석을-위한-기본단위--fundamental-units-in-circuit-analysis-and-design)
    - [키르히호프의 법칙 | Kirchhoff's Law](#키르히호프의-법칙--kirchhoffs-law)
    - [노드 해석법 | Node Analysis](#노드-해석법--node-analysis)
    - [메시 해석법 | Mesh Analysis](#메시-해석법--mesh-analysis)
    - [회로 기호 | Electronic Circuit Symbols](#회로-기호--electronic-circuit-symbols)
  - [참고자료 | Reference](#참고자료--reference)

## 용어 | Terminology

| 용어(Terminology) | 설명(Description) | 기호(Symbol) | 단위(Unit) | 공식(Formula) |
|---|---|---|---|---|
| 전하(Charge) | 양성자는 [+] 전하를 띠고, 전자는 [-] 전하를 띠며, 중성자는 전하를 가지지 않음. 자유전자는 전류를 흐르게 해줌<br>Protons carry a [+] charge, electrons carry a [-] charge, and neutrons have no charge. Free electrons enable the flow of current. | Q | [C]coulomb |  |
| 전류(Current) | 전하의 흐름. 전자의 이동을 통해 전기가 흐름<br>Flow of charge. Electricity flows through the movement of electrons. | I | [A]ampere | `I = Q / t` |
| 직류(DC: Direct Current) | 전류의 방향과 크기가 시간에 따라 변하지 않는 전류<br>Current whose direction and magnitude remain constant over time. | I | [A]ampere |  |
| 교류(AC: Alternating Current) | 전류의 방향과 크기가 주기적으로 변하는 전류<br>Current whose direction and magnitude vary periodically. | i | [A]ampere | `i(t) = I_max * sin(ωt)` |
| 전압(Voltage) | 단위 전하량에 의해 변환된 위치 에너지<br>Energy per unit charge converted from position energy. | V | [V]volt | `V = W / Q` |
| 저항(Resistance) | 전류의 흐름에 저항을 가하는 물질의 성질<br>Property of a material that resists the flow of current. | R | [Ω]ohm | `R = V / I` |
| 전도(Conductance) | 전류의 흐름을 용이하게 하는 물질의 성질<br>Property of a material that facilitates the flow of current. | G | [S]siemens (또는 mho) | `G = 1 / R` |
| 전력(Power) | 단위 시간당 소비되는 에너지의 양<br>Amount of energy consumed per unit time. | P | [W]watt | `P = V * I` 또는 `P = I^2 * R` 또는 `P = V^2 / R` |

## 소자 | Element
![소자](./images/circuit/소자.png)

- **수동 소자 | Passive Element**  
  : 전압을 낮춤  
  : Reduces voltage  
  예) 저항(R), 인덕터(L), 커패시터(C)  
  ex) Resistor (R), Inductor (L), Capacitor (C)
  ```
  - 인덕터(Inductor) : 전자기장을 이용한 전자부품, 과도전류의 변화를 이용해서 전압의 변화를 유도해내는 전자부품

  - 커패시터(Capacitor) : 전자회로에서 전기를 일시적으로 저장하는 장치
    축전기 혹은 콘덴서(Condenser)라고도 부름
  ```
  => 인덕터 : **전압**의 변화에 저항  
  => 커패시터 : **전류**의 변화에 저항  
  하여 급격한 변화를 막아주는 역할을 함.

---
- **능동 소자 | Active Element**  
  : 전압을 공급  
  : Supplies voltage  
  예) 건전지  
  ex) Battery

---
- **저항 소자 | Resistor**  
![저항값 읽기](./images/circuit/저항값.png)

## 전원 | Source

- **독립 전원 | Independent Source**  
  : 다른 소자의 에너지 값에 상관없이 그 자체가 가지고 있는 에너지를 직접 혹은 독립적으로 공급하는 전원  
  : A power source that provides energy directly or independently, regardless of other elements' energy values  
  예) 건전지  
  ex) Battery

  ![독립 전원](./images/circuit/독립전원.png)

---

- **종속 전원 | Dependent Source**  
  : 다른 소자의 상태에 따라 그 전압이나 전류의 값을 조정하여 에너지를 공급하는 전원  
  : A power source that supplies energy by adjusting its voltage or current based on the state of other elements  
  예) 전압 제어 전압원 (VCVS), 전류 제어 전압원 (CCVS)  
  ex) Voltage-controlled voltage source (VCVS), Current-controlled voltage source (CCVS)

  ![종속 전원](./images/circuit/종속전원.png)

  ![종속 전원 종류](./images/circuit/종속전원%20종류.png)

## 전압 | Voltage
접지 연결 상태에 따라 분류

- **접지 전압 | Grounded Voltage**  
  : 접지에 직접 연결되어 있는 전압으로, 접지지점의 전압 값을 0으로 했을 때의 상대적인 단자 전압 값  
  : Voltage directly connected to ground, relative to the voltage at the ground point when its value is considered as 0.  
  예) 가정용 전원, 계측기 전원  
  ex) Household power, instrument power

----

- **부유 전압 | Floating Voltage**  
  : 직접 접지에 연결되어 있지 않은 전압   
  : Voltage not directly connected to ground.   
  예) 건전지  
  ex) Battery

### 옴의 법칙 | Ohm's Law
- 직류 및 실효치 (DC & RMS: Root Mean Square) : V = IR
- 교류 (AC) : v = iR

## 회로 해석 | Circuit Analysis

### 회로해석을 위한 기본단위 | Fundamental Units in Circuit Analysis and Design

- **노드(Node)**  
  : 여러 개의 소자가 만나는 지점  
  : Point connected with several Elements

- **폐루프(Closed Loop)**  
  : 여러 개의 소자가 연결되어 하나의 닫힌 고리를 만드는 것  
  : Path formed by interconnected components creating a closed loop

- **메시(Mesh)**  
  : 폐루프 중에서 그 루프 안에 또 다른 폐루프가 없는 가장 작은 단위   
  : The smallest closed loop in a circuit where no other loops exist within it

### 키르히호프의 법칙 | Kirchhoff's Law
- **KCL - 키르히호프의 전류 법칙 | Kirchhoff's Current Law**   
  : 노드에 기반(Based on Node)  

  -> 노드로 흐르는 전류가 0이 되어야 함.  
  -> the currents flowing into a node must add up to zero.  
  *노드 기준 들어오는 전류의 합 = 나가는 전류의 합*

- **KVL - 키르히호프의 전압 법칙 | Kirchhoff's Voltage Law**   
  : 폐회로에 기반(Based on Closed Loop) 

  -> 회로의 루프를 돌면서 각 소자의 전압의 합이 0이 되어야 함.  
  -> if you travel around any loop in a circuit, the voltages across the elements add up to zero.

### 노드 해석법 | Node Analysis
- 슈퍼 노드 | Super Node  
  : 부유전압전원이 연결되어 있는
노드가 2개 일 때 슈퍼노드를 이용

1. 슈퍼노드에 속해 있는 전압원은 당연히 node의 전압을 구하기 위해 필요한 관계식을 제공해준다.
2. 슈퍼노드 그 자체로는 전압을 가지지 않는다. (계산된 값은 O)
3. 슈퍼노드 회로를 해석하기 위해서는 KCL과 KVL 둘 다를 사용해야 한다.

### 메시 해석법 | Mesh Analysis

- 슈퍼 메시 | Super Mesh  
  : 전류전원이 두 개의 메시 사이에 있는
경우 슈퍼 메시를 이용 (KVL 적용X)

### 회로 기호 | Electronic Circuit Symbols

- 저항 기호

![저항 기호](./images/circuit/저항%20기호.png)

- 커패시터,인덕터 기호

![커패시터,인덕터 기호](./images/circuit/커패시터,%20인덕터%20기호.png)

- 트랜지스터 기호

![트랜지스터 기호](./images/circuit/트랜지스터%20기호.png)

- 다이오드 기호

![다이오드 기호](./images/circuit/다이오드%20기호.png)

- 도선, 회로 반환 기호

![도선, 회로 반환 기호](./images/circuit/도선,%20회로%20반환%20기호.png)

- 소스 기호

![소스 기호](./images/circuit/소스%20기호.png)

- 스위치 기호

![스위치 기호](./images/circuit/스위치%20기호.png)

## 참고자료 | Reference
- [삼성 파운드리 용어사전](https://semiconductor.samsung.com/kr/support/tools-resources/dictionary/)
- [최윤식. 『IT CookBook, 기초 회로이론(개정판):선형회로해석의 기본 원리』. 한빛아카데미, 2012](https://www.hanbit.co.kr/store/books/look.php?p_code=B5575452421)
- [Khan Academy-Electrical engineering-circuit engineerign](https://www.khanacademy.org/science/electrical-engineering/ee-circuit-analysis-topic/ee-dc-circuit-analysis/a/ee-circuit-analysis-overview)
