
1. Build IDPs coil Library from PDB database <br>
2. MaxCycle <- 10 <br>
3. AminoAcidsList <- {Ala, Arg, ... Thr, Val} <br>
4. for i in AminoAcidList <br>
5. 		CMAP_i <- 0 <br>
6. 		j <- 0 <br>
7.   	while j < MaxCycle <br>
8.    	MD_Rama_i <- MD simualtion <br>
9.    	BM_rama_i <- IDPs coil Library <br>
10.    	if RMSp(MD_Rama_i, BM_rama_i) >= 0.1%，then <br>
11.     	CMAP_i <- CMAP_i + delta(MD_Rama_i, BM_rama_i) <br>
12.    	else <br>
13.     	CMAP_i <- CMAP_i <br>
14.    		j <- j + 1 <br>
15.    <br>
      
