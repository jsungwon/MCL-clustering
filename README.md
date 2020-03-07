# Introduction
This c++ code performes MCL clustering for constructing orthologous gene family cluster.
The original algorithm and idea is described in [AJ. *et. al.*](https://www.ncbi.nlm.nih.gov/pubmed/11917018).

# Compile
This code uses open MP library.
```bash
g++ Clustering_Score_MP.cpp -o <your_excutable_file_name>
```

# Usage

## Inputs
You need to put three parameters.
### 1. File Table
#### Format
```
ProteinID1\tProteinID2\tDistance_Score
```
### 2. Number of Thread
   default thread is 1
### 3. Inflation number
   default inflation number is 1.5

## Run
``` bash
Clustering_Score_MP <file_table> <N_thread> <N_Inflation> > out.txt
```

# Citation
1. The whale shark genome reveals how genomic and physiological properties scale with body size
2.  An efficient algorithm for large-scale detection of protein families.
