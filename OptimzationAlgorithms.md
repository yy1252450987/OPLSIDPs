
1. Build IDPs coil Library from PDB database <br>
2. MaxCycle <- 10 <br>
3. AminoAcidsList <- {Ala, Arg, ... Thr, Val} <br>
4. for i in AminoAcidList <br>
  4.1 CMAP_i <- 0 <br>
  4.2 j <- 0 <br>
  4.3 while j < MaxCycle <br>
     MD_Rama_i <- MD simualtion <br>
    BM_rama_i <- IDPs coil Library <br>
    if RMSp(MD_Rama_i, BM_rama_i) >= 0.1%，then <br>
    CMAP_i <- CMAP_i + delta(MD_Rama_i, BM_rama_i) <br>
    else <br>
      CMAP_i <- CMAP_i <br>
    j <- j + 1 <br>
    <br>
      
