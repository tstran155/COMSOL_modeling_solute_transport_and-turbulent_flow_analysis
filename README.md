# COMSOL_modeling_gas_transport_and-turbulent_flow_analysis





Data input deck

| Name     | Expression      | Value     |  Description     |
| ------------- | ------------- | -------- | --------- |
| V_tot	| 540e-6[m^3]	| 5.4E-4 m³	| System volume |
| V_oil_ini	| 270e-6 [m^3] |	2.7E-4 m³	| Initial volume of oil |
| M_oil	| 0.209[kg/mol]	| 0.209 kg/mol	| Molecular weight of oil |
| m_oil	| (V_oil_ini)*(ro_oil)	| 0.2214 kg	| Mass of oil in the cell |
| P_ini	| 1.01e5[Pa]	| 1.01E5 Pa	| Initial pressure |
| P_set	| 1.39e7[Pa]	| 1.39E7 Pa	| Setting pressure |
| P_inj	| 5.45e6[Pa]	| 5.45E6 Pa	| Injection pressure |
| TK	| 273+50[K]	| 323 K	| System temperature |
| q	| 6.39E-7[m^3/s]	| 6.39E-7 m³/s	| Injection rate |
| A	| 0.00828[m^2]	| 0.00828 m²	| Surface area |
| M_C1	| 0.01604[kg/mol]	| 0.01604 kg/mol	| Molecular weight of gas |
| ro_oil	| 820[kg/m^3]	| 820 kg/m³	| Density of oil |

Geometry

![Geometry](https://user-images.githubusercontent.com/86640902/209020350-a7b6245a-777b-45c9-8286-8179784ca0c6.png)

Surface velocity

![image](https://user-images.githubusercontent.com/86640902/209023584-7cbfe43e-4d45-42a0-a5d9-37900b8e2c1e.png)

Surface concentration

![image](https://user-images.githubusercontent.com/86640902/209023651-0cb2ebe5-e095-41e1-9bd9-f9cdf65746fe.png)

Concentration changes over time at the center point

![image](https://user-images.githubusercontent.com/86640902/209028214-8a301ccb-f133-4c1b-949b-7b758372cb2f.png)

Gas transport during injection processes

![Concentration](https://user-images.githubusercontent.com/86640902/209023203-4f951c5c-2070-406c-b8a9-1de68f5b3a5c.gif)
