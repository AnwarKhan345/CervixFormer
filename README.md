# CervixFormer
A Multi-scale Swin Transformer-based Cervical Pap-Smear WSI Classification Framework

## Abstract:

### Background and Objectives
Cervical cancer affects around 0.5 million women per year, resulting in over 0.3 million fatalities. Therefore, repetitive screening for cervical cancer is of utmost importance. Computer-assisted diagnosis is key for scaling up cervical cancer screening. Current recognition algorithms, however, perform poorly on the whole-slide image (WSI) analysis, fail to generalize for different staining methods and on uneven distribution for subtype imaging, and provide sub-optimal clinical-level interpretations. Herein, we developed CervixFormer—an end-to-end, multi-scale swin transformer-based adversarial ensemble learning framework to assess pre-cancerous and cancer-specific cervical malignant lesions on WSIs.


### Methods
The proposed framework consists of (1) a self-attention generative adversarial network (SAGAN) for generating synthetic images during patch-level training to address the class imbalanced problems; (2) a multi-scale transformer-based ensemble learning method for cell identification at various stages, including atypical squamous cells (ASC) and atypical squamous cells of undetermined significance (ASCUS), which have not been demonstrated in previous studies; and (3) a fusion model for concatenating ensemble-based results and producing final outcomes.


![Swin](https://github.com/AnwarKhan345/CervixFormer/assets/57401537/b6c89ebc-f1b4-482b-96e8-a5cc0f7c5901)

### Results
In the evaluation, the proposed method is first evaluated on a private dataset of 717 annotated samples from six classes, obtaining a high recall and precision of 0.940 and 0.934, respectively, in roughly 1.2 minutes. To further examine the generalizability of CervixFormer, we evaluated it on four independent, publicly available datasets, namely, the CRIC cervix, Mendeley LBC, SIPaKMeD Pap Smear, and Cervix93 Extended Depth of Field image datasets. CervixFormer obtained a fairly better performance on two-, three-, four-, and six-class classification of smear- and cell-level datasets. For clinical interpretation, we used GradCAM to visualize a coarse localization map, highlighting important regions in the WSI. Notably, CervixFormer extracts feature mostly from the cell nucleus and partially from the cytoplasm.


![GradCAM](https://github.com/AnwarKhan345/CervixFormer/assets/57401537/fed523b6-4c21-411c-b4d9-45c6c75b2049)


### Conclusions
In comparison with the existing state-of-the-art benchmark methods, the CervixFormer outperforms them in terms of recall, accuracy, and computing time.

![roc_curves](https://github.com/AnwarKhan345/CervixFormer/assets/57401537/cedff18d-4ed7-4fed-b538-d81e6e74deee)

## Citation:

Khan, A., Han, S., Ilyas, N., Lee, Y. M., & Lee, B. (2023). Cervixformer: Transformer-Based Cervical Pap-Smear WSI Classification Framework. Available at SSRN 4266652.

## Contact

If you have any questions, or comments, or would like to report a bug, please file a Github issue or contact me at anwerkhan345@gmail.com/anwar.khan@kuleuven.be 

