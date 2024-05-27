# Jupyter notebooks

This folder contains all Jupyter notebooks relevant to the integration process. (Note that paths within the notebooks do not correspond with the current repository.) This folder contains the following subfolders:


## 1_preprocessing/

contains a notebook for each atlas, in which the aligned h5 files are shaped with annotations and quality control metrics. This additional information will be used to filter the data and prepare it for subsequent processing. For each h5 file a <sample_name>_preprocessed.h5ad file will be made which contain all necessary annotation for subsequent filtering. Key steps performed here:

  * Doublet detection 
  * Adding quality metrics and mitochondrial gene removal
  
## 2_filtering/

contains a notebook for each atlas, in which various quality control metric values are visualized and data is filtered based on threshold made on the observations/domain knowledge. Key steps performed here:

  * Doublet filtering 
  * UMIs and gene counts filtering 

## 3_normalization/

contains a notebook for each atlas, in which the data is normalized based on sequencing depth and gene length so the cells are comparable. Subsequently dimensional reduction and clustering are performed to visualize samples separately. Key steps performed here:

  * Normalization 
  * Dimensional reduction 
  * Marker genes and property annotation visualizations 

## 4_merging/

contains a notebook for each atlas, in which the different samples within a dataset are merged and visualized. Key steps performed here:

  * Merging 
  * Alignment parameter visualization 

## 5_label_transfer/

contains a notebook used to perform label transferring on the integrated dataset. Key steps performed here:
 
  * Hierarchy tree formation using scHPL
  * Label transfer using K-nearest neighbours

## 6_supp_fig_9/

contains a notebook used to create supplementary figure 9.

