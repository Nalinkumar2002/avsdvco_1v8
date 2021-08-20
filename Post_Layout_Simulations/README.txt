 ==================================== 
 IP Name :avsdvco_1V8
 PDK : Sky130 PDK by Google SkyWater
 ==================================== 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  Name of the author : NALINKUMAR S 
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 --------------------------------->
 To perform Post-Layout Simulations 
 --------------------------------->
 	
 --> In file "avsdvco_1v8_post_layout.cir.out" change the control voltage and transient command to get output for various control voltages.
 --> To get outputs at different control voltages change the transient command according to control voltages given below for perfect output graphs
 
 ---------------------------------------------------
  VCTRL (Control Voltage) |    Transient command
 ---------------------------------------------------
	0.4 V   	  |	tran 10ns 100us
	0.5 V		  |	tran 1ns 5us
	0.6 V		  |	tran 100ps 500ns
	0.7 V		  |	tran 10ps 50ns
	0.8 V		  |	tran 10ps 20ns
	0.9 V  		  |	tran 1ps 10ns
	1.0 V		  |	tran 1ps 5ns
	1.1 V		  |	tran 1ps 5ns
	1.2 V		  |	tran 1ps 5ns
	1.3 V		  |	tran 1ps 5ns
	1.4 V		  |	tran 1ps 5ns
	1.5 V		  |	tran 1ps 5ns
	1.6 V		  |	tran 1ps 5ns
	
 *Note: -> Before performing simulations keep the " sky130_fd_pr " folder in current working directory to avoid errors.
 	-> To get output frequency vs bias voltage plot varry VDD from 1.5 V to 2.0 V @ VCTRL = 0.9 V

 --> After performing all analysis the values are tabulated and output graphs are ploted :
	
	TABLES:
	-------
	-> AVSDVCO_1V8 OUTPUT FREQUENCY VS CONTROL VOLTAGE - avsdvco_1v8_post_layout_table_1.png
	-> AVSDVCO_1V8 BIAS CURRENT VS CONTROL VOLTAGE - avsdvco_1v8_post_layout_table_2.png	
	-> AVSDVCO_1V8 OUTPUT FREQUENCY VS BIAS VOLTAGE - avsdvco_1v8_post_layout_table_3.png
	
	PLOTS:
	------
	-> AVSDVCO_1V8 OUTPUT FREQUENCY VS CONTROL VOLTAGE - avsdvco_1v8_post_layout_output_1.png
	-> AVSDVCO_1V8 BIAS CURRENT VS CONTROL VOLTAGE - avsdvco_1v8_post_layout_output_2.png	
	-> AVSDVCO_1V8 OUTPUT FREQUENCY VS BIAS VOLTAGE - avsdvco_1v8_post_layout_output_3.png
	-> AVSDVCO_1V8 TRANSIENT ANALYSIS @ VCTRL = 0.9 V - avsdvco_1v8_post_layout_output.png
