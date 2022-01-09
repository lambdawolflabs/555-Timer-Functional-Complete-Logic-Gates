# 555-Timer-Functional-Complete-Logic-Gates


Hackaday IO Project Link Here (More details there): https://hackaday.io/project/183516 

For 2021/2022 Hackaday/Digikey 555 Timer Contest: https://hackaday.io/contest/182830-555-timer-contest

**
Overview:**
Purpose: 2 bit ripple-carry adder using nothing but 556s timer chips ( 2bits x (2 XORs + 2 ANDs + 1 OR = 6 + 6 + 2 + 2 + 3) ) = 38 555s or 19 556s. Inputs being dip switches and the outputs being LEDs. 

	A couple of spare 555s for demonstrating various gates individually:
		NOT - 1 555
		AND - 2 555
		NOR - 2 555
		XOR - 6 555
		D Flip Flop (Safe, not edge triggered)    -   Requires 7 555s?

Specs:

	-Room Temp Operation (25C +/-10C) 
	-Powered by bench power supply with binding posts or hooks (reverse protection MOSFET included)
	-NO explicit ESD protection.


Logic Gate Ports:

	<FUNC>_<CMOS or NMOS>_<IN or OUT>_<Boolean Identifier: A B or Y or Q  or Abar  or  Bbar>   
	
	e.g.  AND_CMOS_IN_A   or    INV_CMOS_OUT_ABAR    or   A0_CMOS_IN
	Q is saved for Flip Flops, Y is saved for logic gates


Switches Ports:

	<FUNC>_<PD or PU or CMOS>_<SW or PB>

	e.g. A2_PD_SW  or  Carry_CMOS_SW  or AND_Demo_A_CMOS_SW

LED Ports:

	<FUNC>_<ActiveHigh or ActiveLow>_LED

	e.g. S3_ActiveHigh_LED

Labels:

	For highest level net name:  <FUNC>_Root  e.g. S0_Root  or Cout_Root
