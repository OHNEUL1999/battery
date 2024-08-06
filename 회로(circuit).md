# 회로 | Circuit

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
![소자](./images/소자.png)

- **수동 소자 | Passive Element**  
  : 전압을 낮춤
  : Reduces voltage  
  예) 저항(R), 인덕터(L), 커패시터(C)  
  ex) Resistor (R), Inductor (L), Capacitor (C)

---
- **능동 소자 | Active Element**  
  : 전압을 공급  
  : Supplies voltage  
  예) 건전지  
  ex) Battery

---
- **저항 소자 | Resistor**  
![저항값 읽기](./images/저항값.png)
