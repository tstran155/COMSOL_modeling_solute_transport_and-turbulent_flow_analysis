# COMSOL_modeling_gas_transport_and-turbulent_flow_analysis

COMSOL Multiphysics is capable of modeling and analyzing a wide range of physical phenomena, including the transport of gas into the bulk oil phase during gas injection or CO2 sequestration. This type of phenomenon can occur in a variety of applications, such as in the oil and gas industry, where gas may be injected into an oil and gas reservoirs for storage.


I used the Transport of Diluted Species and Large Eddy Simulation Residual Based Variational Multiscale (LES RBVM) Modules in COMSOL Multiphysics to model the transport of gas into the bulk oil phase during gas injection processes. This model was used to simulate the visualization study of C1/Montney-oil interactions as detailed in the attached article SPE-201109-PA.
Main steps to set up the COMSOL model and perform computation of pressure, velocity and concentration over time are as follows:


1.	The gas and oil phases: Define the properties of the gas and the oil, such as their densities, viscosities, and diffusivities.


2.	The boundary conditions: Specify the boundary conditions of the system and at the inlet of the system such as the gas injection rate and pressure.


3.	The governing equations: Set up the transport equations for the gas and the oil phases.

Here are the data input for the model and some key results.

**Data input deck**

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

**Geometry of the system and boundary conditions**

![Geometry](https://user-images.githubusercontent.com/86640902/209020350-a7b6245a-777b-45c9-8286-8179784ca0c6.png)

**System mesh**

![image](https://user-images.githubusercontent.com/86640902/209035793-a851118e-5062-49fb-9109-b1cb3a2bf08c.png)

**Plot of surface velocity**

![image](https://user-images.githubusercontent.com/86640902/209023584-7cbfe43e-4d45-42a0-a5d9-37900b8e2c1e.png)

**Plot of surface concentration**

![image](https://user-images.githubusercontent.com/86640902/209023651-0cb2ebe5-e095-41e1-9bd9-f9cdf65746fe.png)

**Concentration changes over time at the center point**

There are spikes in the data at times 80 seconds and 310 seconds, which correspond to the appearance of finger-like turbulent flows that can be observed in the animation of the entire gas injection process.

![image](https://user-images.githubusercontent.com/86640902/209028214-8a301ccb-f133-4c1b-949b-7b758372cb2f.png)

**Gas transport during injection processes**

![Concentration](https://user-images.githubusercontent.com/86640902/209023203-4f951c5c-2070-406c-b8a9-1de68f5b3a5c.gif)
