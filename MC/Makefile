test_pp: test_Pythia8	
test_PbPb: test_Hijing	
test_PbPb_central: test_Hijing_central
test_PbPb_semicentral: test_Hijing_semicentral	
test_PbPb_peripheral: test_Hijing_peripheral

test_Pythia8: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode full --nevents 2 --uid 1 --generator Pythia8 --system p-p

test_Muon: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode full,Muon --nevents 2 --uid 1 --generator Pythia6_Perugia2011 --system p-p

test_Rsn001: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode full --nevents 2 --uid 1 --generator Pythia8_Monash2013_Rsn001 --system p-p

### [ALIROOT-6721] [ALIROOT-6722]

Hijing_Rsn002a: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 2 --uid 1 --generator Hijing_Rsn002a --bmin  0 --bmax  5 --system Pb-Pb

Hijing_Rsn002b: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 2 --uid 1 --generator Hijing_Rsn002b --bmin  5 --bmax 11 --system Pb-Pb

Hijing_Rsn002c: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 2 --uid 1 --generator Hijing_Rsn002c --bmin 11 --bmax 15 --system Pb-Pb

### [ALIROOT-6750]

Hijing_Jpsiee001: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 1 --uid 1 --generator Hijing_Jpsiee001 --system Pb-Pb  --bmin 11 --bmax 15

###

EPOSLHC_pp: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode full --nevents 1 --uid 1 --generator EPOSLHC

### [ALIROOT-XXXX] Pb-Pb preparations

Hijing: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 1 --uid 1 --generator Hijing


Hijing_central: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 1 --uid 1 --generator Hijing --bmin 0 --bmax 5


Hijing_semicentral: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 1 --uid 1 --generator Hijing --bmin 5 --bmax 11


Hijing_peripheral: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 245064 --mode full --nevents 1 --uid 1 --generator Hijing --bmin 11 --bmax 15


EPOSLHC_PbPb: clean
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode ocdb
	$(ALIDPG_ROOT)/bin/aliroot_dpgsim.sh --run 225106 --mode full --nevents 1 --uid 1 --generator EPOSLHC

###

clean:
	rm -rf *~ *.root *.log *.inp *.dat stress* validation* GRP input
