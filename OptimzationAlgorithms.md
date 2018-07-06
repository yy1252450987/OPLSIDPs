
Build IDPs coil Library from PDB database <br>
MaxCycle <- 10 <br>
AminoAcidsList <- {Ala, Arg, ... Thr, Val} <br>
for i in AminoAcidList <br>
  <\t>CMAP_i <- 0 <br>
  j <- 0 <br>
  while j < MaxCycle <br>
    MD_Rama_i <- MD simualtion <br>
    BM_rama_i <- IDPs coil Library <br>
    if RMSp(MD_Rama_i, BM_rama_i) >= 0.1% <br>
      CMAP_i <- CMAP_i + delta(MD_Rama_i, BM_rama_i) <br>
    else <br>
      CMAP_i <- CMAP_i <br>
    j <- j + 1 <br>
    <br>
      
