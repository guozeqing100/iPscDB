# iPscDB
![17293d1c48780bb6fb9901ad9d14ac19](https://github.com/user-attachments/assets/7bffed40-96b3-4340-a57f-3b3023d4aadc)
- System website: https://www.tobaccodb.org/ipscdb/homePage
- Demo video: https://www.tobaccodb.org/server_ipscdb/source_material/other/ipscdb.mp4
# Overview
## Welcome to iPscDB
iPscDB has already integrated 1,118,601 cells from 182 samples of 9 plants, covering 12 tissues and 6 sequencing platforms. The scRNA-seq data from different studies were analyzed and integrated on study, tissue, and species levels with a standardized pipeline. iPscDB provides three different levels of atlas for the collected six plant species:whole plant level, tissue level and study level. iPscDB is accessible at https://www.tobaccodb.org/ipscdb/homePage.
# Datasets and usage
iPscDB mainly provides six modules:
Browser - Including meta information, sample QC, sanmple intergration, and download options for both .rds file formats for our datasets.
Atlas - Including 38 species atlases and 59 tissue atlaes, each of which can be viewed and downloaded, and contains a variety of displays。
Marker - Including general and classic two types of markers, and the data can be found in the summary and details marker tables .
Search - Three seacrch methods, include marker gene search, cell type search and sequence search using Blast.
Tools - Including four tools: Cross-species gene expression, Developmental trajectory, electronic Single-Cell Pictograph, Plant Cell-Blast.
Pipeline - Including three parts: Job submission, Pipeline models, Result managerment.

## A.Datasets
PscDB downloaded SRA data from databases such as NCBI, ENI and GSA for 946 experiments in 113 projects, covering 38 plant species (including model plants such as Arabidopsis, rice, maize, soybean, tomato and tobacco), and we aligned the original data with reference genomes. At the same time, two different types of cell markers were collected: experimentally validated marker genes, and differentially expressed genes of specific cells identified by scRNA-seq. In order to ensure the unity of tissue and cell types, we normalized tissue and cell type names into standard bibliographies based on the Plant Ontology database.
<img width="1268" height="345" alt="1" src="https://github.com/user-attachments/assets/2c9ccb5c-100f-46a2-8876-cec72746e7a2" />
## B.Usage
### Home
The home page provides a global view of 38 plant tissue maps, and by clicking on hyperlinks embedded in web images, you can quickly explore the cell maps of entire plants and tissues. The tissue chart of different plants can be switched by clicking on the picture in the upper right corner. The Tissue chart makes it easy to quickly browse the map of listed cell types, and a detailed interface for painting the map can be accessed by clicking the tissue icon.
<img width="1555" height="679" alt="2" src="https://github.com/user-attachments/assets/033be0e1-f8dc-4f86-a9a8-b371e6cfbe63" />
### Browse
In this module, iPscDB provides all data statistics, details of each data set, and data integration operations. The data statistics show the number of species, data sets, cell maps, number of genes, number of cell markers and so on.
<img width="1231" height="641" alt="3" src="https://github.com/user-attachments/assets/39fcd0ea-d75a-4f87-b751-f176f65bfe26" />
In addition, meta information is provided for each data set, Information includes dataset, BioProject, Species, Tissue, Treatment, Genotype, Libraries, AGE, Samples, Cells and Publication, Users can use browser buttons or download datasets.
<img width="1221" height="1014" alt="4" src="https://github.com/user-attachments/assets/0e546d83-9e57-42ba-9979-24407bffb0ca" />
### Atlas
In this module, we provide three types of Atlas：Species atlas, Tissue atlas, Spatial Atlas. The interface provides browsing and downloading functions, and the data displays species name, tissue name, number of data sets, number of cell types and number of cells.
<img width="1224" height="242" alt="5" src="https://github.com/user-attachments/assets/113014b4-47ad-4cb9-a29b-88ae828a3681" />
<img width="1219" height="249" alt="6" src="https://github.com/user-attachments/assets/6acdec29-94de-4b15-8aed-f800afda5f61" />
<img width="1238" height="252" alt="7" src="https://github.com/user-attachments/assets/1dc90893-d14f-47a2-8097-d11b9f5a06a6" />
In the exploreIn the explore interface, the gene retrieval function could be found in the upper part, the Umap or tSNE infographic of Atlas, cell number in each cell type, Gene Number in each cell(the number of genes expressed by each cell in each cell type), cell to cell similarity, number of expressed gene(the number of genes expressed in each cell type), and the cell markers and sample tables were displayed below.
<img width="1254" height="728" alt="8" src="https://github.com/user-attachments/assets/a5002c7f-0d74-4059-a3cc-b8e7866e42f7" />
### Marker 
Here, iPscDB offers an informative module that provides marker gene information for each cell type across various species. Users can easily select a cell type using either the Bar chart or the Tree list. In the specific cell type panel, scPlantDB offers informative visualizations in the form of word clouds that display the number of source datasets for each marker gene. Additionally, users can access meta-information about the cell type, including the number of plant species and tissues that share this cell type.
<img width="1267" height="987" alt="9" src="https://github.com/user-attachments/assets/a47c284d-a7dc-4779-9c32-4d7c693ed6f1" />
<img width="1828" height="1186" alt="10" src="https://github.com/user-attachments/assets/2c8152a9-f5b5-4179-ac43-0834a701737c" />
In the tables of marker genes, the times of the gene are displayed, which has been reported in a certain cell type, and whether the gene has been validated experimentally. If it is a classic gene, its pentagram will light up. At the same time, in the details table, the P-value and fold-change value of each marker gene are displayed.
<img width="912" height="1095" alt="11" src="https://github.com/user-attachments/assets/84930e5d-86c7-47f1-b5da-9c69917997d7" />
<img width="915" height="887" alt="12" src="https://github.com/user-attachments/assets/d0010270-5e16-47b2-952d-a97850fa5a24" />
### Search
Users can easily access the search panel in iPscDB by simply clicking on the search icon in the navigation bar. The search panel offers two efficient methods to help users quickly find the desired information: marker/cell type name searching and sequence searching. The marker/cell type name search allows users to enter keywords related to the cell type or marker they are looking for, including both exact matches and partial matches of markers description. On the other hand, the sequence search mainly relies on BLAST algorithm, allowing users to input a nucleotide or amino acid sequence and compare it against sequences of species in the database. Both searching methods offer convenient and precise results to meet users’ various research needs.
<img width="1269" height="735" alt="13" src="https://github.com/user-attachments/assets/6a5cc97e-8652-42c6-b706-14666f1cc635" />
### Pipeline User Guide
Upon registration and login, users can access the iPscDB online single-cell data analysis pipeline. The pipeline consists of three main components: Job Submission, Analysis Modules, and Browse Results.
#### Job Submission
iPscDB supports job submission for two data types: FASTQ files and Cell Ranger outputs. The complete workflow includes Cell Ranger analysis, Quality Control (QC), Data Processing, Clustering, and Cell Annotation. The platform supports both One-step mode (using all default parameters) and Step-by-Step mode (allowing users to manually adjust parameters), as detailed below:
##### Start with FASTQ files
This module supports raw sequencing data from 10x Genomics, including Index files (I1, I2) and Sequence files (R1, R2). For detailed file format specifications, please refer to the official 10x Genomics website. After entering the job name and selecting the reference species and tissue type, users will be directed to the data input interface, as shown in the figure below.
<img width="1267" height="524" alt="14" src="https://github.com/user-attachments/assets/acd8391f-6645-4374-9f90-04e59a0d227f" />
Note: The input files must strictly adhere to specific naming conventions. Please refer to the example files for the correct format. Once data upload is complete, proceed immediately to the Cell Ranger analysis, which will run with default parameters. The subsequent analysis workflow is described in the following sections.
<img width="1269" height="358" alt="15" src="https://github.com/user-attachments/assets/70934131-da5b-496f-bfb3-1a00f2e2f33b" />
##### Start with cellranger files
This module supports output data from Cell Ranger analysis. These files are typically located in the /Cellranger_Sample/outs/ filtered_feature_bc_matrix directory and must include barcodes.tsv.gz, features.tsv.gz, and matrix.mtx.gz. After entering the job name, reference species, and tissue type, users can access the data input interface, as shown below.
<img width="1267" height="474" alt="16" src="https://github.com/user-attachments/assets/9fc35fa9-dd47-49f7-8d6f-5054fcd0c8cf" />
Upon completion of data upload and loading, specific parameters for Sample QC will be displayed. The algorithm for automatic parameter setting is defined as follows. nFeature_RNA.cutmax: qnorm(0.95, mean = mean(nFeature_RNA), sd = sd(nFeature_RNA) nFeature_RNA.cutmin： max(200, qnorm(0.05, mean = mean(nFeature_RNA), sd = sd(nFeature_RNA))
<img width="1268" height="434" alt="17" src="https://github.com/user-attachments/assets/aedfa370-4608-491a-a029-38d7a0ca9387" />
Users can modify these parameters here and run the subsequent quality control steps to obtain the corresponding results.
<img width="1878" height="1236" alt="18" src="https://github.com/user-attachments/assets/7b71b28d-1e01-423d-b491-40fe13dfcf24" />
After verifying the quality control data, users can proceed to Data Processing, which includes Normalization, Scaling, and Finding Variable Features. The relevant parameters are shown below.
<img width="1670" height="1000" alt="19" src="https://github.com/user-attachments/assets/c6101b5c-88ea-4670-8ecb-25986ca71411" />
Users can consult the official Seurat website for details on parameter settings, and then submit the job to reach the following stage:
<img width="1088" height="406" alt="20" src="https://github.com/user-attachments/assets/8d69c8ac-f061-4df4-a922-c25dec092ede" />
After adjusting the Cluster resolution, users can perform clustering.
<img width="1268" height="672" alt="21" src="https://github.com/user-attachments/assets/94ffe175-ac23-40df-badf-6274303ddf5d" />
iPscDB provides an online image editing feature here. Clicking it allows users to customize the UMAP plot, including Basic Settings and Graphic Settings.
<img width="642" height="924" alt="22" src="https://github.com/user-attachments/assets/8fbfd74c-11b2-489b-9b1a-ef6313256c93" />
At this stage, iPscDB provides options to download Cluster marker genes and the Cluster gene expression matrix. Users can use iPscDB's Cell Type Predictor tool with gene expression matrices from other sources for prediction. Alternatively, to use the built-in annotation pipeline, proceed to the next step. Clicking "Next" will initiate annotation using the Plant CellID tool, generating results such as annotation plots, cell type marker gene lists, and marker gene heatmaps.
<img width="1268" height="629" alt="23" src="https://github.com/user-attachments/assets/d309104d-0ebb-4cda-b62c-0b247350b2e7" />
<img width="1265" height="577" alt="24" src="https://github.com/user-attachments/assets/88c5ce63-7bfa-4224-b36d-f38f8a89bc67" />
<img width="1269" height="770" alt="25" src="https://github.com/user-attachments/assets/8b499b3d-129c-4443-a5c2-8048348f5f38" />
#### Analysis Modules
The Analysis Modules section consists of the four distinct steps found in the pipeline. Each module can be run independently, however, users must prepare the input files in the specific formats required by each module.
<img width="1269" height="302" alt="26" src="https://github.com/user-attachments/assets/99792a8e-7b94-4fe1-8f2f-163e2d0bc74d" />
<img width="1268" height="702" alt="27" src="https://github.com/user-attachments/assets/d9411117-26c3-4cfb-b480-99399983c775" />
<img width="1268" height="558" alt="28" src="https://github.com/user-attachments/assets/4cc4636a-6198-4953-84f2-2bb45336852c" />
<img width="1268" height="597" alt="29" src="https://github.com/user-attachments/assets/bc5e5467-d067-440c-859b-54c9dfed5423" />
#### Result Management
All jobs can be managed in the results interface. Under the Operation column, users can choose to view logs, inspect job results, or delete jobs, as shown in the figure below.
<img width="1265" height="537" alt="30" src="https://github.com/user-attachments/assets/3f24bec3-4fa6-4e0e-8798-ad2cc35933cc" />
### Tools
iPscDB provides a wealth of online single-cell data analysis capabilities, includes Cross-species gene expression, Developmental trajectory, electronic Single-Cell Pictograph and Plant Cell Blast annotation with multiple references tools, users can choose the appropriate tools according to the needs of data analysis for analysis.
<img width="619" height="714" alt="31" src="https://github.com/user-attachments/assets/ec6393e6-40fb-44f8-b816-8b3f3bfb1750" />
<img width="1244" height="654" alt="32" src="https://github.com/user-attachments/assets/60401029-37dd-4efc-a633-b4ecd599093c" />
<img width="953" height="804" alt="33" src="https://github.com/user-attachments/assets/75d464dc-4983-4433-a8e0-e73ed7893b28" />
<img width="1245" height="581" alt="34" src="https://github.com/user-attachments/assets/1926edb5-ae35-4e0a-b60d-3156d5a9a006" />
## Contact us
Comments and suggestions are welcomed
If you meet any troubles or find any bugs when you visit iPscDB, please email to penglu2004@hotmail.com, peijiancao@163.com
Address: No.2 Fengyang Street, High-Tech Zone, Zhengzhou, P. R, 450001
## Submit data
Welcome to submit single-cell data to the iPscDB
If you have a group of single-cell data in plants and would like to submit them to iPscDB.Please email your expression matrix data to penglu2004@hotmail.com, peijiancao@163.com with the following format:
- 1.RDS file
- 2.Barcodes, Features, and Matrix files
- 3.H5 file
- 4.Reference genome version
Sinale-cell data will be uploaded after manuscript acceptance. All submissions will be really appreciated!
