## 1. Description
*  The EF_LDOR01 is a positive low dropout regulator for output of 1.8 V. It is capable of supplying 100 mA of output current with a dropout voltage of 650 mV. Low operating quiescent current of 115 µA is consumed at no load current. Moreover, it provides a standard fixed output voltage of 1.8V which is a good choice for logic power supply. The EF_LDOR01 requires an output capacitance of 47 μF with a wide range of ESR (0.1 Ω to 0.5 Ω) for stability. Output capacitors of this size are typically included in most regulator designs.The functional block diagram is illustrated in Figure 1.

<img src="https://github.com/Ahmedredamohamed2022/EF_LDOR01/blob/main/docs/_static/figure1.functionalblockdiagram.png" width="300" height="250">

*Figure 1. Functional Block Diagram*

## 2. Features
* 100mA Output Current Capability.
* Standard Fixed Output Voltage of 1.8 V.
* Low Dropout Voltage: 650 mV at 100 mA.
* Stable with Output Capacitor of 47 µF.
  - CAP ALUM 47UF 20% 35V SMD.
* Low Supply Current of 115 µA (No Load).
* Low Temperature Coefficient 125 ppm/°C.
* 0.016 V/V Line Regulation at 100 mA.
*	0.0083 mV/mA Load Regulation at 3.3 V.
*	Power Supply Ripple Rejection of 38.9 dB.
*	Startup time of 450 µs at rising time of 100 µs.

## 3. Applications
*	3.3V to 1.8V Logic Power Supply 

## 4. Pin Configuration and Functions

* Corresponding to the Block Diagram of the EF_LDOR01, each pin name with its function is described in Table 1. Moreover, typical application of the EF_LDOR01 configuration is presented in Figure 2, where, Co=47µF, ESR=0.1Ω, RB1=450 KΩ, RB2=300 KΩ, and Trim[6]=3.3 V. Min RL is  18 Ω to provide Max load current of 100 mA.

*Table 1. Pin Configuration and Functions*
<img src="https://github.com/Ahmedredamohamed2022/EF_LDOR01/blob/main/docs/_static/table1.png" width="1000" height="200">

<img src="https://github.com/Ahmedredamohamed2022/EF_LDOR01/blob/main/docs/_static/figure2.typical_application.png"  width="300" height="200">

*Figure 2. Typical Application*

## 5. Electrical Characteristics

* The post-layout simulation results of the proposed EF_LDOR01 are listed in Table 2. Those parameters are reported at Temp.=27°C,Co=47µF, ESR=0.1Ω, RB1=450 KΩ, RB2=300 KΩ, Trim[6]=3.3 V. 

*Table 2. Electrical Characteristics*
<img src="https://github.com/Ahmedredamohamed2022/EF_LDOR01/blob/main/docs/_static/table2.png" width="1000" height="800">

## 6. Typical Performance Curves

* The proposed EF_LDOR01 has been designed and simulated using open-source tools with SkyWater technology. Herein, [XSCHEM](https://xschem.sourceforge.io/stefan/index.html) is a schematic capture program that provides a graphical method of the electronic schematic circuit, easily. [NGSPICE](http://ngspice.sourceforge.net/download.html) is an open-source spice simulator. It is exploied to simulate and verify the designed circuit. Layout of the EF_DACR0801 is implemented using [MAGIC 8.3](http://opencircuitdesign.com/magic/) and for design rule check (DRC) as well. However, [NETGEN](http://opencircuitdesign.com/netgen/) is used for comparing netlists of the layout and schematic, known as layout vs schamtc (LVS). [PYTHON](https://www.python.org/) can be integrated with NGSPICE simulator for data manipulation/analysis of the simulation result.

#### Next, typical perofmane curves of the EF_LDOR01 post-layout simulations are presented. 
As depicted in Figure 3 (a), EF_LDOR01's output is ploted with sweeping the input voltgae from 0V to 5V at different levels of load currents. Besides, the dorpout voltages are calculated at different levels of load currents, then plotted as shown in Figure 3 (b).

<img src="https://github.com/Ahmedredamohamed2022/EF_LDOR01/blob/main/docs/_static/figure3.(a)%20Output%20Voltage%20vs%20Input%20Voltage.png" width="800" height="500">

*(a)*

<img src="https://github.com/Ahmedredamohamed2022/EF_LDOR01/blob/main/docs/_static/figure3.%20(b)dropout_voltage_%20vs_load%20current..png" width="300" height="200">

*(b)*

*Figure 3. (a) Output Voltage vs Input Voltage, (b) Dropout Voltage vs Load Current.*


