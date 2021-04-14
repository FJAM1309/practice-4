transcript on
if {[file exists rtl_work]} {
	vdel -lib rtl_work -all
}
vlib rtl_work
vmap work rtl_work

vlog -vlog01compat -work work +incdir+D:/Quartus/intelFPGA_lite/p4 {D:/Quartus/intelFPGA_lite/p4/TopModule.v}
vlog -vlog01compat -work work +incdir+D:/Quartus/intelFPGA_lite/p4 {D:/Quartus/intelFPGA_lite/p4/Debouncing.v}
vlog -vlog01compat -work work +incdir+D:/Quartus/intelFPGA_lite/p4 {D:/Quartus/intelFPGA_lite/p4/DivF.v}
vlog -vlog01compat -work work +incdir+D:/Quartus/intelFPGA_lite/p4 {D:/Quartus/intelFPGA_lite/p4/PeriodCounter.v}

vlog -vlog01compat -work work +incdir+D:/Quartus/intelFPGA_lite/p4 {D:/Quartus/intelFPGA_lite/p4/TopModule_tb.v}

vsim -t 1ps -L altera_ver -L lpm_ver -L sgate_ver -L altera_mf_ver -L altera_lnsim_ver -L fiftyfivenm_ver -L rtl_work -L work -voptargs="+acc"  TopModule_tb

add wave *
view structure
view signals
run -all
