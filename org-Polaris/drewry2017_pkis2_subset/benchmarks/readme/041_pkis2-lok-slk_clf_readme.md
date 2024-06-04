![molprop](https://storage.googleapis.com/polaris-public/icons/icons8-fox-60-kinases.png)

### Background
**LOK** (STK10) is involved in multiple signaling pathways, including the p38 mitogen-activated protein kinase (MAPK) pathway. 
research on STK10 as a therapeutic target was still in its early stages. Preclinical studies in cell lines and animal models might have been conducted to investigate the effects of STK10 inhibition on tumor growth and other cellular processes

**SLK** (STE20-like kinase) is a serine/threonine kinase that belongs to the STE20 family of kinases. It plays a role in various cellular processes, including cell cycle progression, cytoskeletal organization, and cell migration. 

### Benchmarking

**SLK** and **STK10** are serine/threonine kinases whose major known function is activating the ERM (ezrin/radixin/moesin) proteins by phosphorylation on a conserved threonine residue near the C-terminus (moesin Thr558). Inhibition of STK10/SLK appears to primarily affect cell migration by suppressing p38 MAPK signaling and attenuating ERM protein activation. This potential therapeutic approach warrants further exploration for its effectiveness in the treatment of diseases characterized by abnormal cell migration, such as certain cancers. 


**The goal** of this benchmark is to perform a multitask, which is to the best predictive model for 
- Dual inhibition on LOK and SLK 
- Optimization of the bioactivity % inhibition.
- Discovery of potential hits in new chemical space.

## Description of readout 
- **Readouts**: `CLASS_LOK`, `CLASS_SLK`
- **Bioassay readout**: percentage of inhnibition.
- **Threshold**: > 80
- **Optimization objective**: postive label (1)
- **Number of data points**: train: 508 test: 132


### Data resource: 
- **Reference**: [PKIS2](https://pubmed.ncbi.nlm.nih.gov/26501955)

### Train/test split
Given the benchmarking goal, a scaffold-based splitting approach was applied to ensure training and test sets contain distinct chemical structures while maintaining the diversity of scaffolds.

**Distribution of the train/test in the chemical space**
![image](![molprop](https://storage.googleapis.com/polaris-public/icons/icons8-fox-60-kinases.png)

### Background
**LOK** (STK10) is involved in multiple signaling pathways, including the p38 mitogen-activated protein kinase (MAPK) pathway. 
research on STK10 as a therapeutic target was still in its early stages. Preclinical studies in cell lines and animal models might have been conducted to investigate the effects of STK10 inhibition on tumor growth and other cellular processes

**SLK** (STE20-like kinase) is a serine/threonine kinase that belongs to the STE20 family of kinases. It plays a role in various cellular processes, including cell cycle progression, cytoskeletal organization, and cell migration. 

### Benchmarking

**SLK** and **STK10** are serine/threonine kinases whose major known function is activating the ERM (ezrin/radixin/moesin) proteins by phosphorylation on a conserved threonine residue near the C-terminus (moesin Thr558). Inhibition of STK10/SLK appears to primarily affect cell migration by suppressing p38 MAPK signaling and attenuating ERM protein activation. This potential therapeutic approach warrants further exploration for its effectiveness in the treatment of diseases characterized by abnormal cell migration, such as certain cancers. 


**The goal** of this benchmark is to perform a multitask, which is to the best predictive model for 
- Dual inhibition on LOK and SLK 
- Optimization of the bioactivity % inhibition.
- Discovery of potential hits in new chemical space.

## Description of readout 
- **Readouts**: `CLASS_LOK`, `CLASS_SLK`
- **Bioassay readout**: percentage of inhnibition.
- **Threshold**: > 80
- **Optimization objective**: postive label (1)
- **Number of data points**: train: 508 test: 132


### Data resource: 
- **Reference**: [PKIS2](https://pubmed.ncbi.nlm.nih.gov/26501955)

### Train/test split
Given the benchmarking goal, a scaffold-based splitting approach was applied to ensure training and test sets contain distinct chemical structures while maintaining the diversity of scaffolds.

**Distribution of the train/test in the chemical space**
![image](https://storage.googleapis.com/polaris-public/datasets/kinases/lok_slk/figures/drewry_lok_slk_v1_tnse_scaffold_split.png)


## Related links
The full curation and creation process is documented -> [notebook](https://github.com/polaris-hub/polaris-recipes/blob/main/org-Polaris/drewry2017_pkis2_subset/01_pkis2_kinase_data_curation.ipynb)