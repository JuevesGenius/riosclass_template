RTLPATH = ../rtl/lab_1/src \
	../rtl/lab_1/src/cache \
	../rtl/lab_1/src/cache/cacheblock \
	../rtl/lab_1/src/core_empty \
	../rtl/lab_1/src/core_empty/lsu \
	../rtl/lab_1/src/core_empty/pipeline \
	../rtl/lab_1/src/core_empty/units \
	.

RTLFILE += $(foreach p,$(RTLPATH),$(wildcard $(p)/*.v $(p)/*.sv))
CFILE = plug.cpp

VCSFLAG = -full64 +v2k -kdb -debug_access+all +define+DUMPON+CPLUG \
	-sverilog +vcs+lic+wait +vc+list +vpi \
	-timescale=1ns/1ps -v2k_generate +incdir+../rtl/lab_1/src


compile:
	vcs $(VCSFLAG) $(RTLFILE) $(CFILE) -top tb_hehe


run:
	$(shell if [ ! -d log ]; then mkdir log; fi;)
	./simv 2>&1 | tee run.log

all: hex compile run

clean:
	rm -rf $(filter-out $(wildcard *.v *.sv *.py *.cpp) makefile isa log,$(wildcard *))
	rm -rf isa/hex/*.hex
	rm -rf temp
