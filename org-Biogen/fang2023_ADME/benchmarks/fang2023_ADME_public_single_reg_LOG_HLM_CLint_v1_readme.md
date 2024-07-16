![ADME](https://storage.googleapis.com/polaris-public/icons/icons8-whale-96-ADME.png) 

## Background

The goal of assessing ADME properties is to understand how a potential drug candidate interacts with the human body, encompassing absorption, distribution, metabolism, and excretion. This knowledge is crucial for evaluating the drug's efficacy, safety, and clinical potential, ultimately guiding drug development towards optimal therapeutic outcomes. [Fang et al. (2023)](https://doi.org/10.1021/acs.jcim.3c00160) disclosed DMPK datasets collected over 20 months, covering six ADME in vitro endpoints: human and rat liver microsomal stability, MDR1-MDCK efflux ratio, solubility, and human and rat plasma protein binding. The dataset includes between 885 and 3,087 measurements for each corresponding endpoint.

## Benchmarking
**The goal** of this benchmark is to perform a single task, which is to have the best predictive model for human liver microsomal stability. 


## Description of readout 
- **Readouts**: `LOG HLM_CLint (mL/min/kg)`
- **Bioassay readout**: Intrinsic clearance
- **Optimization objective**: Higher value

## Molecule data resource:
**Reference**: https://doi.org/10.1021/acs.jcim.3c00160

## Train/test split
In this benchmark set, the same train/test sets as in the fang2023 paper were used for the 6 endpoints: human and rat liver microsomal stability, MDR1-MDCK efflux ratio, solubility, and human and rat plasma protein binding, respectively. 
See more details at https://github.com/molecularinformatics/Computational-ADME/tree/main/MPNN.

**Distribution of the train/test in the chemical space**
![image](https://storage.googleapis.com/polaris-public/datasets/ADME/fang2023/figures/fang2023_ADME_public_v1_HLM_tsne_fang2023split.png)


## Related links
The full curation and creation process is documented [here](https://github.com/polaris-hub/polaris-recipes/blob/main/01_ADME).
