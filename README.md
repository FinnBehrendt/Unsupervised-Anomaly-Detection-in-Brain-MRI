# Unsupervised-Anomaly-Detection-in-Brain-MRI

In this repository, we provide a collection of peer reviewed literature about Unsupervised Anomaly Detection (UAD) in brain MRI.
We will try to keep the repository up-to-date and welcome contributions of others when a new matching paper is published or has completed peer-review.

#### Citation
```python
@article{TBD
}
```


## Contents
- [Open Source Datasets](#Open-Source-Datasets)
- [Papers](#papers)
  - [Feature-Based Approaches](#Feature-based)
  - [Reconstruction-based Approaches](#Reconstruction-based)
    - [Auto-Encoder](#AE)
    - [Variational Autoencoder](#VAE)
    - [Generative Adversarial Networks](#GAN)
    - [Diffusion Models](#DM)
    - [Other models](#others)   
  - [Synthetic Anomalies](#ssl)
## Open Source Datasets 
- ***Individual Brain Charting (IBC) dataset***\
 **Individual Brain Charting dataset extension, second release of high-resolution fMRI data for cognitive mapping** \
  *Pinho, Ana Lu\'isa, Amadon, Alexis, Gauthier, Baptiste, Clairis, Nicolas, Knops, Andr\'e, Genon, Sarah, Dohmatob, Elvis, Torre, Juan Jes\'us, Ginisty, Chantal, Becuwe-Desmidt, S\'everine, Roger, S\'everine, Lecomte, Yann, Berland, Val\'erie, Laurier, Laurence, Joly-Testault, V\'eronique, M\'ediouni-Cloarec, Ga\"elle, Doubl\'e* \
  [2020] [Scientific data, 2020]<br>
  [[Paper](https://doi.org/10.1038/s41597-020-00670-4)]
  [[Access Data](https://project.inria.fr/IBC/ibc-in-a-nutshell/)]
- ***Calgary-Campinas-359 (CC359) dataset***\
 **An open, multi-vendor, multi-field-strength brain MR dataset and analysis of publicly available skull stripping methods agreement** \
  *Souza, Roberto, Lucena, Oeslle, Garrafa, Julia, Gobbi, David, Saluzzi, Marina, Appenzeller, Simone, Rittner, Let\'icia, Frayne, Richard, Lotufo, Roberto* \
  [2018] [NeuroImage, 2018]<br>
  [[Paper](https://doi.org/10.1016/j.neuroimage.2017.08.021)]
  [[Access Data](https://www.ccdataset.com/download)]

- ***Parkinson Progression Marker Initiative (PPMI) dataset*** \
  **The Parkinson Progression Marker Initiative (PPMI)** \
  [2011] [Progress in neurobiology, 2011]<br>
  [[Paper](https://doi.org/10.1016/j.pneurobio.2011.09.005)]
  [[Access Data](https://www.ppmi-info.org/access-data-specimens/download-data)]
  
- ***Developing Human Connectome Project (dHCP) dataset*** \
  **A dedicated neonatal brain imaging system** \
  *Hughes, Emer J., Winchman, Tobias, Padormo, Francesco, Teixeira, Rui, Wurie, Julia, Sharma, Maryanne, Fox, Matthew, Hutter, Jana, Cordero-Grande, Lucilio, Price, Anthony N., Allsop, Joanna, Bueno-Conde, Jose, Tusor, Nora, Arichi, Tomoki, Edwards, A. D., Rutherford, Mary A., Counsell, Serena J., Hajnal, Joseph V.* \
  [2017] [Magnetic resonance in medicine, 2017]<br>
  [[Paper](https://doi.org/10.1002/mrm.26462)]
  [[Access Data](https://www.developingconnectome.org/data-release/second-data-release/)]
- ***Information eXtraction from Images (IXI) dataset*** \
  *Biomedical Image Analysis Group* \
  [[Access Data](https://brain-development.org/ixi-dataset/)]

- ***The Human Connectome Project (HPC) dataset***\
  **The Human Connectome Project: a data acquisition perspective** \
  *van Essen* \
  [2012] [NeuroImage, 2012]<br>
  [[Paper](https://doi.org/10.1016/j.neuroimage.2012.02.018)]
  [[Access Data](https://www.humanconnectome.org/study/hcp-young-adult/data-releases)]
  
- ***The Alzheimer's Disease Neuroimaging Initiative (ADNI) dataset*** \
  **The Alzheimer's Disease Neuroimaging Initiative 3: Continued innovation for clinical trial improvement** \
  *Weiner, Michael W., Veitch, Dallas P., Aisen, Paul S., Beckett, Laurel A., Cairns, Nigel J., Green, Robert C., Harvey, Danielle, Jack, Clifford R., Jagust, William, Morris, John C., Petersen, Ronald C., Salazar, Jennifer, Saykin, Andrew J., Shaw, Leslie M., Toga, Arthur W., Trojanowski, John Q.* \
  [2017] [Alzheimer's, 2017]<br>
  [[Paper](https://pubmed.ncbi.nlm.nih.gov/27931796/)]
  [[Access Data](https://adni.loni.usc.edu/data-samples/access-data/)]

- ***The Open Access Series of Imaging Studies (OASIS) dataset*** \
  **OASIS-3: Longitudinal neuroimaging, clinical, and cognitive dataset for normal aging and Alzheimer's disease** \
  *LaMontagne, Pamela J., Keefe, Sarah, Lauren, Wallace, Xiong, Chengjie, Grant, Elizabeth A., Moulder, Krista L., Morris, John C., Benzinger, Tammie L.S., Marcus, Daniel S.* \
  [2018] [Alzheimer's, 2018]<br>
  [[Paper](https://www.readcube.com/articles/10.1101/2019.12.13.19014902)]
  [[Access Data](https://www.oasis-brains.org)]

- ***The Cambridge Centre for Ageing and Neuroscience (Cam-CAN) dataset*** \
  **The Cambridge Centre for Ageing and Neuroscience (Cam-CAN) data repository: Structural and functional MRI, MEG, and cognitive data from a cross-sectional adult lifespan sample** \
  *Taylor, Jason R., Williams, Nitin, Cusack, Rhodri, Auer, Tibor, Shafto, Meredith A., Dixon, Marie, Tyler, Lorraine K., Cam-Can, Henson, Richard N.* \
  [2017] [NeuroImage, 2017]<br>
[[Paper](https://pubmed.ncbi.nlm.nih.gov/26375206/)]
[[Access Data](https://camcan-archive.mrc-cbu.cam.ac.uk/dataaccess/)]
- ***UK biobank (UKB) dataset*** \
  **UK biobank: an open access resource for identifying the causes of a wide range of complex diseases of middle and old age** \
  *Sudlow, Cathie, Gallacher, John, Allen, Naomi, Beral, Valerie, Burton, Paul, Danesh, John, Downey, Paul, Elliott, Paul, Green, Jane, Landray, Martin, Liu, Bette, Matthews, Paul, Ong, Giok, Pell, Jill, Silman, Alan, Young, Alan, Sprosen, Tim, Peakman, Tim, Collins, Rory* \
  [2015] [PLoS medicine, 2015]<br>
  [[Paper](https://pubmed.ncbi.nlm.nih.gov/25826379/)]
  [[Access Data](https://biobank.ndph.ox.ac.uk/showcase/field.cgi?id=54)]

- ***fastMRI (fMRI) dataset*** \
  **fastMRI: An Open Dataset and Benchmarks for Accelerated MRI** \
  *Zbontar, Jure, Knoll, Florian, Sriram, Anuroop, Murrell, Tullie, Huang, Zhengnan, Muckley, Matthew J., Defazio, Aaron, Stern, Ruben, Johnson, Patricia, Bruno, Mary, Parente, Marc, Geras, Krzysztof J., Katsnelson, Joe, Chandarana, Hersh, Zhang, Zizhao, Drozdzal, Michal, Romero, Adriana, Rabbat, Michael, Vincent, Pascal, Yakubova, Nafissa, Pinkerton, James, Wang, Duo, Owens, Erich, Zitnick, C. Lawrence, Recht, Michael P., Sodickson, Daniel K., Lui, Yvonne W.* \
  [2019] [ArXiv] \
  [[Paper](https://arxiv.org/pdf/1811.08839.pdf)]
  [[Access Data](https://fastmri.med.nyu.edu)]
  

- ***The Maryland Magnets Prospective (MagNets) dataset***\
   **Investigation of Prognostic Ability of Novel Imaging Markers for Traumatic Brain Injury (TBI)** \
  *Gullapalli, Rao P.* \
  [2011][Defense Technical Information Center]\
  [[Report](https://apps.dtic.mil/sti/pdfs/ADA577060.pdf)]
  [[Access Data](https://fitbir.nih.gov/study_profile/314)]
  
- ***The Multiple Sclerosis data set from the University Hospital of Ljubljana (MSLUB) dataset*** \
  **A novel public MR image dataset of multiple sclerosis patients with lesion segmentations based on multi-rater consensus** \
  *Lesjak, \vZiga, Galimzianova, Alfiia, Koren, Ale\vs, Lukin, Matej, Pernu\vs* \
  [2018] [Neuroinformatics, 2018]<br>
  [[Paper](https://pubmed.ncbi.nlm.nih.gov/29103086/)]
  [[Access Data](https://lit.fe.uni-lj.si/en/raziskave/viri/3D-MR-MS/)]
  
- ***The Multiple Sclerosis Segmentation Challenge (MSSEG) dataset***\
  **Objective Evaluation of Multiple Sclerosis Lesion Segmentation using a Data Management and Processing Infrastructure** \
  *Commowick, Olivier, Istace, Audrey, Kain, Micha\"el, Laurent, Baptiste, Leray, Florent, Simon, Mathieu, Pop, Sorina Camarasu, Girard, Pascal, Am\'eli, Roxana, Ferr\'e* \
  [2018] [Scientific Reports, 2018]<br>
[[Paper](https://www.nature.com/articles/s41598-018-31911-7)]
[[Access Data](https://shifts.grand-challenge.org/datasets/)]

- ***The Anatomical Tracings of Lesions After Stroke (ATLAS) data set (V1, V2)***\
  **A large, curated, open-source stroke neuroimaging dataset to improve lesion segmentation algorithms** \
  *Liew, Sook-Lei, Lo, Bethany P., Donnelly, Miranda R., Zavaliangos-Petropulu, Artemis, Jeong, Jessica N., Barisano, Giuseppe, Hutton, Alexandre, Simon, Julia P., Juliano, Julia M., Suri, Anisha, others* \
  [2022] [Scientific data, 2022]<br>
  [[Paper](https://www.nature.com/articles/sdata201811)]
  [[Access Data](https://fcon_1000.projects.nitrc.org/indi/retro/atlas.html)]

- ***The white matter hyperintensities (WMH) dataset*** \
  **Standardized assessment of automatic segmentation of white matter hyperintensities and results of the WMH segmentation challenge** \
  *Kuijf, Hugo J., Biesbroek, J. Matthijs, de Bresser, Jeroen, Heinen, Rutger, Andermatt, Simon, Bento, Mariana, Berseth, Matt, Belyaev, Mikhail, Cardoso, M. Jorge, Casamitjana, Adria, others* \
  [2019] [IEEE transactions on medical imaging, 2019]<br>
   [[Paper](https://pubmed.ncbi.nlm.nih.gov/30908194/)]
  [[Access Data](https://dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/AECRSD)]
  
- ***The ischemic stroke lesion segmentation (ISLES) dataset*** \
  **ISLES 2015 - A public evaluation benchmark for ischemic stroke lesion segmentation from multispectral MRI** \
  *Maier, Oskar, Menze, Bjoern H., von der Gablentz, Janina, Hani, Levin, Heinrich, Mattias P., Liebrand, Matthias, Winzeck, Stefan, Basit, Abdul, Bentley, Paul, Chen, Liang, Christiaens, Daan, Dutil, Francis, Egger, Karl, Feng, Chaolu, Glocker, Ben, Goetz, Michael, Haeck, Tom, Halme, Hanna-Leena, Havaei, Mohammad, Iftekharuddin, Khan M., Jodoin, Pierre-Marc, Kamnitsas, Konstantinos, Kellner, Elias, Korvenoja, Antti, Larochelle, Hugo, Ledig, Christian, Lee, Jia-Hong, Maes, Frederik, Mahmood, Qaiser, Maier-Hein, Klaus H., McKinley, Richard, Muschelli, John, Pal, Chris, Pei, Linmin, Rangarajan, Janaki Raman, Reza, Syed M. S., Robben, David, Rueckert, Daniel, Salli, Eero, Suetens, Paul, Wang, Ching-Wei, Wilms, Matthias, Kirschke, Jan S., Kr Amer* \
  [2017] [Medical Image Analysis, 2017]<br>
 [[Paper](https://linkinghub.elsevier.com/retrieve/pii/S1361-8415(16)30126-8)]
[[Access Data](www.isles-challenge.org)]

- ***The centre for clinical brain sciences (CBS) dataset*** \
  **A structural and functional magnetic resonance imaging dataset of brain tumour patients** \
  *Pernet, Cyril R., Gorgolewski, Krzysztof J., Job, Dominic, Rodriguez, David, Whittle, Ian, Wardlaw, Joanna* \
  [2016] [Scientific data, 2016]<br>
  [[Paper](https://doi.org/10.1038/sdata.2016.3)]
[Access Data](https://reshare.ukdataservice.ac.uk/851861/)]

- ***The Multimodal Brain Tumor Segmentation (BraTS) datasets (2021 version)*** \
  **The rsna-asnr-miccai brats 2021 benchmark on brain tumor segmentation and radiogenomic classification** \
  *Baid, Ujjwal and Ghodasara, Satyam and Mohan, Suyash and Bilello, Michel and Calabrese, Evan and Colak, Errol and Farahani, Keyvan and Kalpathy-Cramer, Jayashree and Kitamura, Felipe C. and Pati, Sarthak and others* \
  [2021][ArXiv] \
  [[Paper](https://arxiv.org/abs/2107.02314)]
  [Access Data](https://www.med.upenn.edu/cbica/brats2021/)]
## Papers 

### Feature based 

- **Modeling normal brain asymmetry in MR images applied to anomaly detection without segmentation and data annotation** \
  *Martins, Samuel, Barbara Caroline Benato, Bruna Ferreira Silva, Clarissa Lyn Yasuda, Alexandre Xavier Falc\~ao* \
  [2019]  [SPIE] \
  [[Paper](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/10950/2512873/Modeling-normal-brain-asymmetry-in-MR-images-applied-to-anomaly/10.1117/12.2512873.full)]
  
- **Regularized siamese neural network for unsupervised outlier detection on brain multiparametric magnetic resonance imaging: Application to epilepsy lesion screening** \
  *Alaverdyan, Zaruhi, Jung, Julien, Bouet, Romain, Lartizien, Carole* \
  [2020] [Medical Image Analysis, 2020]<br>
  [[Paper](https://www.sciencedirect.com/science/article/pii/S1361841519301562)]
  
- **SS3D: Unsupervised Out-of-Distribution Detection and Localization for Medical Volumes** \
  *Doorenbos, Lars, Sznitman, Raphael, M\'arquez-Neila, Pablo* \
  [2021][MICCAI - Biomedical Image Registration, Domain Generalisation and Out-of-Distribution Analysis]\
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-97281-3_17)]
  [[Code](https://github.com/LarsDoorenbos/SS3D)]
  
- **Anomaly Detection via Context and Local Feature Matching** \
  *Kascenas, Antanas, Young, Rory, Jensen, Bjorn Sand, Pugeault, Nicolas, O'Neil, Alison Q.* \
  [2022] [2022 IEEE 19th International Symposium on Biomedical Imaging (ISBI), 2022]<br>
  [[Paper](https://doi.org/10.1109/ISBI52829.2022.9761524)]
  
- **Unsupervised anomaly localization with structural feature-autoencoders** \
  *Meissen, Felix, Paetzold, Johannes, Kaissis, Georgios, Rueckert, Daniel* \
  [2022][MICCAI - Brainlesion: Glioma, Multiple Sclerosis, Stroke and Traumatic Brain Injuries] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-33842-7_2)]
  [[Code](https://github.com/FeliMe/feature-autoencoder)]
  
- **Brain Subtle Anomaly Detection Based on Auto-Encoders Latent Space Analysis: Application To De Novo Parkinson Patients** \
  *Pinon, Nicolas, Oudoumanessah, Geoffroy, Trombetta, Robin, Dojat, Michel, Forbes, Florence, Lartizien, Carole* \
  [2023] [2023 IEEE 20th International Symposium on Biomedical Imaging (ISBI), 2023]<br>
  [[Paper](https://doi.org/10.1109/ISBI53787.2023.10230351)]

- **One-Class SVM on siamese neural network latent space for Unsupervised Anomaly Detection on brain MRI White Matter Hyperintensities** \
  Pinon, Nicolas, Trombetta, Robin, Lartizien Carole* \
  [2023] [Medical Imaging with Deep Learning, 2023]<br>
  [[Paper](https://openreview.net/forum?id=_c9r6-HCEaN)]


- **Feature-Based Pipeline for Improving Unsupervised Anomaly Segmentation on Medical Images** \
  *Frolova, Daria, Katrutsa, Aleksandr, Oseledets, Ivan* \
  [2023] [MICCAI - Uncertainty for Safe Utilization of Machine Learning in Medical Imaging]<br>
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-44336-7_12)]
  [[Code](https://github.com/2na-97/CGV_MOOD2022/)]


- **Encoder-Decoder Contrast for Unsupervised Anomaly Detection in Medical Images** \
  *Guo, Jia, Lu, Shuai, Jia, Lize, Zhang, Weihang, Li, Huiqi* \
  [2023] [IEEE transactions on medical imaging, 2023]<br>
  [[Paper](https://doi.org/10.1109/TMI.2023.3327720)]
  [[Code](https://github.com/guojiajeremy/EDC)]
  
- **Contrastive Representations for Unsupervised Anomaly Detection and Localization** \
  *Lüth, Carsten, Zimmerer, David, Koehler, Gregor, Jaeger, Paul, Isensee, Fabian, Maier-Hein, Klaus* \
  [2023] [BVM, 2023]<br>
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-658-41657-7_54)]
  
### Reconstruction based

- AE
  - **Bayesian Skip-Autoencoders for Unsupervised Hyperintense Anomaly Detection in High Resolution Brain Mri** \
  *Baur, Christoph, Wiestler, Benedikt, Albarqouni, Shadi, Navab, Nassir* \
  [2020] [2020 IEEE 17th International Symposium on Biomedical Imaging (ISBI), 2020]<br>
  [[Paper](https://doi.org/10.1109/ISBI45749.2020.9098686)]

  - **Scale-Space Autoencoders for Unsupervised Anomaly Segmentation in Brain MRI** \
  *Baur, Christoph, Wiestler, Benedikt, Albarqouni, Shadi, Navab, Nassir* \
  [2020] [Medical Image Computing and Computer Assisted Intervention -- MICCAI 2020, 2020]<br>
  [[Paper](https://doi.org/10.1007/978-3-030-59719-1{\textunderscore )]

  - **Modeling Healthy Anatomy with Artificial Intelligence for Unsupervised Anomaly Detection in Brain MRI** \
  *Baur, Christoph, Wiestler, Benedikt, Muehlau, Mark, Zimmer, Claus, Navab, Nassir, Albarqouni, Shadi* \
  [2021] [Radiology: Artificial Intelligence, 2021]<br>
  [[Paper](https://doi.org/10.1148/ryai.2021190169)]

  - **Denoising Autoencoders for Unsupervised Anomaly Detection in Brain MRI** \
  *Kascenas, Antanas, Pugeault, Nicolas, O'Neil, Alison Q.* \
  [2022] [Proceedings of The 5th International Conference on Medical Imaging with Deep Learning, 2022]<br>
  [[Paper](https://proceedings.mlr.press/v172/kascenas22a.html)]
  [[Code](https://github.com/AntanasKascenas/DenoisingAE)]

  - **Unsupervised Detection of Lesions in Brain MRI using constrained adversarial auto-encoders** \
  *Chen, Xiaoran, Konukoglu, Ender* \
  [2022] [Medical Imaging with Deep Learning, 2022]<br>
  [[Paper](https://arxiv.org/abs/1806.04972)]
  [[Code](https://github.com/aubreychen9012/cAAE)]


  - **Federated disentangled representation learning for unsupervised brain anomaly detection** \
  *Bercea, Cosmin I., Wiestler, Benedikt, Rueckert, Daniel, Albarqouni, Shadi* \
  [2022] [Nature Machine Intelligence, 2022]<br>
  [[Paper](https://doi.org/10.1038/s42256-022-00515-2)]
  [[Code](https://github.com/albarqounilab/FedDis-NMI)]

  - **A dual autoencoder and singular value decomposition based feature optimization for the segmentation of brain tumor from MRI images** \
  *Aswani, K., Menaka, D.* \
  [2021] [BMC Medical Imaging, 2021]<br>
  [[Paper](https://bmcmedimaging.biomedcentral.com/articles/10.1186/s12880-021-00614-3)]

  - **Unsupervised Anomaly Detection in 3D Brain MRI Using Deep Learning with Impured Training Data** \
  *Behrendt, Finn, Bengs, Marcel, Rogge, Frederik, Kruger, Julia, Opfer, Roland, Schlaefer, Alexander* \
  [2022] [2022 IEEE 19th International Symposium on Biomedical Imaging (ISBI), 2022]<br>
  [[Paper](https://doi.org/10.1109/ISBI52829.2022.9761443)]

  - **Dual-distribution discrepancy with self-supervised refinement for anomaly detection in medical images** \
  *Cai, Yu, Chen, Hao, Yang, Xin, Zhou, Yu, Cheng, Kwang-Ting* \
  [2023] [Medical Image Analysis, 2023]<br>
  [[Paper](https://doi.org/10.1016/j.media.2023.102794)]
  [[Code](https://github.com/caiyu6666/DDAD-ASR)]

  - **Outlier detection in multimodal MRI identifies rare individual phenotypes among more than 15,000 brains** \
  *Ma, Zhiwei, Reich, Daniel S., Dembling, Sarah, Duyn, Jeff H., Koretsky, Alan P.* \
  [2022] [Human brain mapping, 2022]<br>
  [[Paper](https://pubmed.ncbi.nlm.nih.gov/34957633/)]

  - **Subtle anomaly detection: Application to brain MRI analysis of de novo Parkinsonian patients** \
  *Mu\~noz-Ram\'irez, Ver\'onica, Kmetzsch, Virgilio, Forbes, Florence, Meoni, Sara, Moro, Elena, Dojat, Michel* \
  [2022] [Artificial Intelligence in Medicine, 2022]<br>
  [[Paper](https://www.sciencedirect.com/science/article/pii/S0933365722000161)]

  - **Unsupervised anomaly detection in brain MRI: Learning abstract distribution from massive healthy brains** \
  *Luo, Guoting, Xie, Wei, Gao, Ronghui, Zheng, Tao, Chen, Lei, Sun, Huaiqiang* \
  [2023] [Computers in Biology and Medicine, 2023]<br>
  [[Paper](https://www.sciencedirect.com/science/article/pii/S0010482523000756)]


- VAE
  - **Context-encoding Variational Autoencoder for Unsupervised Anomaly  Detection** \
  *Zimmerer, David, Kohl, Simon, Petersen, Jens, Isensee, Fabian, Maier-Hein, Klaus* \
  [2019] [International Conference on Medical Imaging with Deep Learning (MIDL), 2019]<br>
  [[Paper](https://arxiv.org/pdf/1907.12258)]

  - **Unsupervised Anomaly Localization Using Variational Auto-Encoders** \
  *Zimmerer, David, Isensee, Fabian, Petersen, Jens, Kohl, Simon, Maier-Hein, Klaus* \
  [2019] [Medical Image Computing and Computer Assisted Intervention -- MICCAI 2019, 2019]<br>
  [[Paper](https://arxiv.org/abs/1907.02796)]
  [[Code](https://github.com/MIC-DKFZ/vae-anomaly-experiments)]

  - **Predictable Uncertainty-Aware Unsupervised Deep Anomaly Segmentation** \
  *Sato, Kazuki, Hama, Kenta, Matsubara, Takashi, Uehara, Kuniaki* \
  [2019] [2019 International Joint Conference on Neural Networks (IJCNN 2019), 2019]<br>
  [[Paper](https://doi.org/10.1109/IJCNN.2019.8852144)]

  - **Unsupervised lesion detection via image restoration with a normative prior** \
  *Chen, Xiaoran, You, Suhang, Tezcan, Kerem Can, Konukoglu, Ender* \
  [2020] [Medical Image Analysis, 2020]<br>
  [[Paper](https://doi.org/10.1016/j.media.2020.101713)]
  [[Code](https://github.com/yousuhang/Unsupervised-Lesion-Detection-via-Image-Restoration-with-a-Normative-Prior)]

  - **Tumor Detection in Brain MRIs by Computing Dissimilarities in the Latent Space of a Variational AutoEncoder** \
  *Albu, Alexandra, Enescu, Alina, Malag\`o* \
  [2020] [Proceedings of the Northern Lights Deep Learning Workshop, 2020]<br>
  [[Paper](https://doi.org/10.7557/18.5172)]

  - **Brain Lesion Detection Using A Robust Variational Autoencoder and Transfer Learning** \
  *Akrami, Haleh, Joshi, Anand A., Li, Jian, Aydore, Sergul, Leahy, Richard M.* \
  [2020] [IEEE 17th International Symposium on Biomedical Imaging, 2020]<br>
  [[Paper](https://doi.org/10.1109/isbi45749.2020.9098405)]

  - **Unsupervised pathology detection in medical images using conditional variational autoencoders** \
  *Uzunova, Hristina, Schultz, Sandra, Handels, Heinz, Ehrhardt, Jan* \
  [2019] [International journal of computer assisted radiology and surgery, 2019]<br>
  [[Paper](https://doi.org/10.1007/s11548-018-1898-0)]

  - **Leveraging 3d Information In Unsupervised Brain Mri Segmentation** \
  *Lambert, Benjamin, Louis, Maxime, Doyle, Senan, Forbes, Florence, Dojat, Michel, Tucholka, Alan* \
  [2021] [2021 IEEE 18th International Symposium on Biomedical Imaging (ISBI), 2021]<br>
  [[Paper](https://doi.org/10.1109/ISBI48211.2021.9433894)]

  - **Constrained unsupervised anomaly segmentation** \
  *Silva-Rodr\'iguez, Julio, Naranjo, Valery, Dolz, Jose* \
  [2022] [Medical Image Analysis, 2022]<br>
  [[Paper](https://www.sciencedirect.com/science/article/pii/S1361841522001736)]
  [[Code](https://github.com/jusiro/constrained_anomaly_segmentation/)]

  - **StRegA: Unsupervised anomaly detection in brain MRIs using a compact context-encoding variational autoencoder** \
  *Chatterjee, Soumick, Sciarra, Alessandro, D\"unnwald, Max, Tummala, Pavan, Agrawal, Shubham Kumar, Jauhari, Aishwarya, Kalra, Aman, Oeltze-Jafra, Steffen, Speck, Oliver, N\"urnberger, Andreas* \
  [2022] [Computers in Biology and Medicine, 2022]<br>
  [[Paper](https://www.sciencedirect.com/science/article/pii/S0010482522008010)]
  [[Code](https://github.com/soumickmj/strega)]

  - **The OOD Blind Spot of Unsupervised Anomaly Detection** \
  *Matth\"aus Heer, Janis Postels, Xiaoran Chen, Ender Konukoglu, Shadi Albarqouni* \
  [2021] [Medical Imaging with Deep Learning, 2021]<br>
  [[Paper](https://proceedings.mlr.press/v143/heer21a.html)]

  - **Generalizing Unsupervised Anomaly Detection: Towards Unbiased Pathology Screening** \
  *Bercea, Cosmin, Benedikt Wiestler, Daniel Rueckert, Julia A Schnabel* \
  [2023] [Medical Imaging with Deep Learning, 2023]<br>
  [[Paper](https://openreview.net/forum?id=8ojx-Ld3yjR)]
  [[Code](https://github.com/ci-ber/RA)]

  - **Three-dimensional deep learning with spatial erasing for unsupervised anomaly segmentation in brain MRI** \
  *Bengs, Marcel, Behrendt, Finn, Kr\"uger, Julia, Opfer, Roland, Schlaefer, Alexander* \
  [2021] [International journal of computer assisted radiology and surgery, 2021]<br>
  [[Paper](https://doi.org/10.1007/s11548-021-02451-9)]

  - **Unsupervised anomaly detection in 3D brain MRI using deep learning with multi-task brain age prediction** \
  *Marcel Bengs, Finn Behrendt, Max-Heinrich Laves, Julia Kr\"uger, Roland Opfer, Alexander Schlaefer* \
  [2022] [Medical Imaging 2022: Computer-Aided Diagnosis, 2022]<br>
  [[Paper](https://doi.org/10.1117/12.2608120)]

  - **Capturing Inter-Slice Dependencies of 3D Brain MRI-Scans for Unsupervised Anomaly Detection** \
  *Finn Behrendt, Marcel Bengs, Debayan Bhattacharya, Julia Kr\"uger, Roland Opfer, Alexander Schlaefer* \
  [2022] [Medical Imaging with Deep Learning, 2022]<br>
  [[Paper](https://openreview.net/forum?id=db8wDgKH4p4)]

  - **On the Pitfalls of Using the Residual Error as Anomaly Score** \
  *Meissen, Felix, Wiestler, Benedikt, Kaissis, Georgios, Rueckert, Daniel* \
  [[Paper](https://arxiv.org/pdf/2202.03826)]
  [[Code](https://github.com/FeliMe/residual-score-pitfalls)]

  - **Unsupervised Brain Anomaly Detection and Segmentation with Transformers** \
  *Pinaya, Walter Hugo Lopez, Tudosiu, Petru-Daniel, Gray, Robert, Rees, Geraint, Nachev, Parashkev, Ourselin, S\'ebastien, Cardoso, M. Jorge* \
  [2021] [Proceedings of the Fourth Conference on Medical Imaging with Deep Learning, 2021]<br>
  [[Paper](https://proceedings.mlr.press/v143/pinaya21a.html)]
  [[Code](https://github.com/Project-MONAI/GenerativeModels)]

  - **Unsupervised abnormality detection in neonatal MRI brain scans using deep learning** \
  *Raad, Jad Dino, Chinnam, Ratna Babu, Arslanturk, Suzan, Tan, Sidhartha, Jeong, Jeong-Won, Mody, Swati* \
  [2023] [Scientific reports, 2023]<br>
  [[Paper](https://doi.org/10.1038/s41598-023-38430-0)]
  [[Code](https://github.com/jraad/unsupervised_neonatal_anomaly_detection)]


- GAN
  - **Deep Autoencoding Models for Unsupervised Anomaly Segmentation in Brain MR Images** \
  *Baur, Christoph, Wiestler, Benedikt, Albarqouni, Shadi, Navab, Nassir* \
  [2019] [Brainlesion: Glioma, Multiple Sclerosis, Stroke and Traumatic Brain Injuries, 2019]<br>
  [[Paper](https://doi.org/10.1007/978-3-030-11723-8{\textunderscore )]

  - **SteGANomaly: Inhibiting CycleGAN Steganography for Unsupervised Anomaly Detection in Brain MRI** \
  *Baur, Christoph, Graf, Robert, Wiestler, Benedikt, Albarqouni, Shadi, Navab, Nassir* \
  [2020] [Medical Image Computing and Computer Assisted Intervention -- MICCAI 2020, 2020]<br>
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-59713-9_69)]

  - **Reversing the Abnormal: Pseudo-Healthy Generative Networks for Anomaly Detection** \
  *Bercea, Cosmin I., Wiestler, Benedikt, Rueckert, Daniel, Schnabel, Julia A.* \
  [2020] [Medical Image Computing and Computer Assisted Intervention -- MICCAI 2020] <br>
  [[Paper](https://arxiv.org/pdf/2303.08452.pdf)]
  [[Code](https://github.com/ci-ber/PHANES)]

  - **MADGAN: unsupervised medical anomaly detection GAN using multiple adjacent brain MRI slice reconstruction** \
  *Han, Changhee, Rundo, Leonardo, Murao, Kohei, Noguchi, Tomoyuki, Shimahara, Yuki, Milacski, Zolt\'an \'Ad\'am, Koshino, Saori, Sala, Evis, Nakayama, Hideki, Satoh, Shin'ichi* \
  [2021] [BMC bioinformatics, 2021]<br>
  [[Paper](https://doi.org/10.1186/s12859-020-03936-1)]

  - **Unsupervised Region-Based Anomaly Detection In Brain MRI With Adversarial Image Inpainting** \
  *Nguyen, Bao, Feldman, Adam, Bethapudi, Sarath, Jennings, Andrew, Willcocks, Chris G.* \
  [2021] [2021 IEEE 18th International Symposium on Biomedical Imaging (ISBI), 2021]<br>
  [[Paper](https://doi.org/10.1109/ISBI48211.2021.9434115)]

  - **An anomaly detection approach to identify chronic brain infarcts on MRI** \
  *van Hespen* \
  [2021] [Scientific Reports, 2021]<br>
  [[Paper](https://www.nature.com/articles/s41598-021-87013-4)]


- DM
  - **Fast Unsupervised Brain Anomaly Detection and Segmentation with Diffusion Models** \
  *Pinaya, Walter H. L., Graham, Mark S., Gray, Robert, Da Costa* \
  [2022] [Medical Image Computing and Computer-Assisted Intervention, MICCAI 2022]<br>
  [[Paper](https://arxiv.org/pdf/2206.03461.pdf)]
  [[Code](https://github.com/Project-MONAI/GenerativeModels)]


  - **Anoddpm: Anomaly detection with denoising diffusion probabilistic models using simplex noise** \
  *Wyatt, Julian, Leach, Adam, Schmon, Sebastian M., Willcocks, Chris G.* \
[Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, ]<br>
[[Paper](https://openaccess.thecvf.com/content/CVPR2022W/NTIRE/papers/Wyatt_AnoDDPM_Anomaly_Detection_With_Denoising_Diffusion_Probabilistic_Models_Using_Simplex_CVPRW_2022_paper.pdf)]
[[Code](https://github.com/Julian-Wyatt/AnoDDPM)]

  - **Patched Diffusion Models for Unsupervised Anomaly Detection in Brain MRI** \
  *Finn Behrendt, Debayan Bhattacharya, Julia Kr\"uger, Roland Opfer, Alexander Schlaefer* \
  [2023] [Medical Imaging with Deep Learning, 2023]<br>
  [[Paper](https://openreview.net/forum?id=O-uZr5S1tJE)]
  [[Code](https://github.com/FinnBehrendt/patched-Diffusion-Models-UAD)]

  - **The role of noise in denoising models for anomaly detection in medical images** \
  *Kascenas, Antanas, Sanchez, Pedro, Schrempf, Patrick, Wang, Chaoyang, Clackett, William, Mikhael, Shadia S., Voisey, Jeremy P., Goatman, Keith, Weir, Alexander, Pugeault, Nicolas, Tsaftaris, Sotirios A., O'Neil, Alison Q.* \
  [2023] [Medical Image Analysis, 2023]<br>
  [[Paper](https://doi.org/10.1016/j.media.2023.102963)]

  - **Mask, Stitch, and Re-Sample: Enhancing Robustness and Generalizability in Anomaly Detection through Automatic Diffusion Models** \
  *Bercea, Cosmin, Michael Neumayr, Daniel Rueckert, Julia A Schnabel* \
  [2023] [ICML 3rd Workshop on Interpretable Machine Learning in Healthcare (IMLH), 2023]<br>
  [[Paper](https://openreview.net/forum?id=kTpafpXrqa)]
  [[Code](https://github.com/ci-ber/autoDDPM)]

  - **Unsupervised Anomaly Detection in Medical Images Using Masked Diffusion Model** \
  *Iqbal, Hasan, Khalid, Umar, Chen, Chen, Hua, Jing* \
  [2023] [MICCAI - Machine Learning in Medical Imaging, 2023]<br>
  [[Paper](https://doi.org/10.1007/978-3-031-45673-2{\textunderscore )]
  [[Code](https://github.com/hasan1292/mDDPM)]

  - **Modality Cycles with Masked Conditional Diffusion for Unsupervised Anomaly Segmentation in MRI** \
  *Liang, Ziyun, Anthony, Harry, Wagner, Felix, Kamnitsas, Konstantinos* \
  [2023] [MICCAI Workshop]<br>
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-47425-5_16)]
  [[Code](https://github.com/ZiyunLiang/MMCCD.)]

  - **Self-supervised diffusion model for anomaly segmentation in medical imaging** \
  *Kumar, Komal, Chakraborty, Snehashis, Roy, Sudipta * \
  [2023] [International Conference on Pattern Recognition and Machine Intelligence]<br>
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-45170-6_37)]
  [[Code](https://github.com/hasan1292/mDDPM)]

- Others
  - **Implicit Field Learning for Unsupervised Anomaly Detection in Medical Images** \
  *Marimont, Naval ,  Tarroni, Giacomo* \
  [2021][Medical Image Computing and Computer-Assisted Intervention, MICCAI 2021] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-87196-3_18)]
  [[Code](https://github.com/snavalm/ifl_unsup_anom_det)]


  - **Challenging Current Semi-supervised Anomaly Segmentation Methods for~Brain MRI** \
  *Meissen, Felix, Kaissis, Georgios, Rueckert, Daniel* \
  [2022] [Brainlesion: Glioma, Multiple Sclerosis, Stroke and Traumatic Brain Injuries, 2022]<br>
  [[Paper](https://arxiv.org/pdf/2109.06023.pdf)]
  [[Code](https://github.com/FeliMe/brain_sas_baseline)]

  - **Autoencoders for unsupervised anomaly segmentation in brain MR images: A comparative study** \
  *Baur, Christoph, Stefan Denner, Benedikt Wiestler, Nassir Navab, Shadi Albarqouni* \
  [2021] [Medical Image Analysis, 2021]<br>
  [[Paper](https://www.sciencedirect.com/science/article/pii/S1361841520303169)]
  [[Code](https://github.com/StefanDenn3r/Unsupervised_Anomaly_Detection_Brain_MRI)]

  - **Unsupervised Pathology Detection: A Deep Dive Into the State of the Art** \
  *Lagogiannis, Ioannis, Meissen, Felix, Kaissis, Georgios, Rueckert, Daniel* \
  [2023] [IEEE transactions on medical imaging, 2023]<br>
  [[Paper](https://doi.org/10.1109/TMI.2023.3298093)]
  [[Code](https://github.com/iolag/UPD_study)]


### Synthetic Anomalies
- **SS3D: Unsupervised Out-of-Distribution Detection and Localization for Medical Volumes** \
  *Doorenbos, Lars, Sznitman, Raphael, M\'arquez-Neila, Pablo* \
  [2021][MICCAI - Biomedical Image Registration, Domain Generalisation and Out-of-Distribution Analysis] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-97281-3_17)]
  [[Code](https://github.com/LarsDoorenbos/SS3D)]

- **AutoSeg - Steering the Inductive Biases for Automatic Pathology Segmentation** \
  *Meissen, Felix, Kaissis, Georgios, Rueckert, Daniel* \
  [2021][MICCAI - Biomedical Image Registration, Domain Generalisation and Out-of-Distribution Analysis] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-97281-3_19)]
  [[Code](https://github.com/felime/autoseg)]
  
- **Self-supervised 3D Out-of-Distribution Detection via Pseudoanomaly Generation** \
  *Cho, Jihoon, Kang, Inha, Park, Jinah* \
  [2021][MICCAI - Biomedical Image Registration, Domain Generalisation and Out-of-Distribution Analysis] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-97281-3_15)]
  
- **Self-supervised Medical Out-of-Distribution Using U-Net Vision Transformers** \
  *Park, Seongjin, Balint, Adam, Hwang, Hyejin* \
  [2021][MICCAI - Biomedical Image Registration, Domain Generalisation and Out-of-Distribution Analysis] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-97281-3_16)]
  
- **MetaDetector: Detecting Outliers by Learning to Learn from Self-supervision** \
  *Tan, Jeremy, Kart, Turkay, Hou, Benjamin, Batten, James, Kainz, Bernhard* \
  [2021][MICCAI - Biomedical Image Registration, Domain Generalisation and Out-of-Distribution Analysis] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-030-97281-3_18)]
  
- **Detecting Outliers with Foreign Patch Interpolation** \  
  *Tan, Jeremy and Hou, Benjamin and Batten, James and Qiu, Huaqi and Kainz, Bernhard* \
  [2022][Machine Learning for Biomedical Imaging] \
  [[Paper](https://arxiv.org/pdf/2011.04197.pdf)]
  [[Code](https://github.com/jemtan/FPI)]

- **Many tasks make light work: Learning to localise medical anomalies from multiple synthetic tasks** \  
  *Baugh, Matthew, Tan, Jeremy, Müller, Johanna, Dombrowski, Mischa, Batten, James, Kainz, Bernhard* \
  [2022][MICCAI] \
  [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-43907-0_16)]
  [[Code](https://github.com/matt-baugh/many-tasks-make-light-work)]

## Acknowledgements
We borrow the structure of this repository from this [awesome repository](https://github.com/amirhossein-kz/Awesome-Diffusion-Models-in-Medical-Imaging/blob/main/README.md?plain=1) 

