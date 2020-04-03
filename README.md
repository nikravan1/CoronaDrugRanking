# CoronaDrugInvestigator


Finding a drug(small molecule) between the existing drug is a fastest way to design a drug for a new disease like Corona. It is named as drug repurposing.Many drugs have been suggested by various individuals and researcher groups for Corona but none of them have been definitively approved for corona treatment.However, due to the urgency of treating patients, many of them have been used in medical centers and have shown their positive effects. ***which drugs have better effects is still unclear***. In this repository, we try to achieve a comparison between these drugs by software simulation and classify the effect of these drugs.
This repository review all of those drug and  examines the docking score between the COVID-19 main protease (as a receptor)  and the drugs (Ligand).Almost all of the alleged drugs are collected here to be investigated with docking software such as Schrödinger, Molegra, Autodock Vina and others.
 There are 13 ligands in the ligand2D folder, including:
 - Atazanavir
- Brilacidin
- Chloroquine
- Darunavir
- Favipiravir
- Galidesivir
- Lopinavir
- Nelfinavir
- Remdesivir
- Ritonavir
- TMC310911
- Triazavirin
- Umifenovir
# Ligand(Drug)-Protein Docking Pipeline
This is the pipeline for checking dock score for each ligand (the molecule of drug ). In this case I use schrodinger software as pipeline base.
- **1-preparing ligand**
  - download 2D file of ligand (sdf format). [from web site like drugbank](https://www.drugbank.ca/)
  - using LigPrep task for transfer 2D to 3D format with minimum energy.
  
   [![Ligand Preparation with LigPrep](https://img.youtube.com/vi/5vO88ui0JdM/0.jpg)](https://www.youtube.com/watch?v=5vO88ui0JdM)
- **2-preparing protein**
    - download protein pdb file ([protein data base](https://www.rcsb.org/)) 
    - Protein prepare with tools like  Protein Preparation Wizard.
  
   [![preparing protein](https://img.youtube.com/vi/YRFROyN88Fw/0.jpg)](https://www.youtube.com/watch?v=YRFROyN88Fw)
- **3-Finding binding site**  
  - for using docking process we must find docking site where the ligand sits inside it. It can be used with 
   Binding Site Detection tools in SCHrodinger Suite.
- **4-Grid Generation**
  - After preparing ligand and protein and finding binding site,It turn to produce grid from protein.
 [![Grid Generation](https://img.youtube.com/vi/_AUKLGtrBR8/0.jpg)](https://www.youtube.com/watch?v=_AUKLGtrBR8)
 - **5-docking operation**
   - It is necessary to do all 4 above step for docking. Use Glide Ligand Docking.
  [![Grid Generation](https://img.youtube.com/vi/htoaov6bQlk/0.jpg)](https://www.youtube.com/watch?v=htoaov6bQlk)
- **6-Viewing Results**
  - you can use any tools for viewing docking score or plot them.
 # Result of Corona virus drug
  


