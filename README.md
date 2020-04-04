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
 # Results
 After doing all the above process on these 13 drug these  Results obtained for docking score(more negative is better) 
 |Rank|Drug Name|Docking Score|
 |:--:|:-------:|:-------:|
 |1|Remdesivir	|-9.34	|
|2|TMC310911	|-7.05	|
|3|Ritonavir	|-6.58	|
|4|Galidesivir|-6.47	|
|5|Brilacidin	|-6.11	|
|6|Lopinavir	|-5.44	|
|7|Darunavir	|-4.99	|
|8|Nelfinavir	|-4.75	|
|9|Atazanavir	|-3.98	|
|10|Favipiravir|-3.61	|
|11|Umifenovir	|-3.53	|
|12|Chloroquine|-3.02	|
|13|Triazavirin|-2.66	|

The above result shows the Remdesivir and TMC310911 are the best drug for corona virus treatment and chloroquine(Trump had suggested it) and Triazavirin are the worst.
 - : exclamation : These results belong to the best site position which is obtained from SiteMap tools in schrodinger software
# Ranking Drug
In this section, all the drugs used to treat covid-19  disease are described (drugbank) in order of their rank.
- ## Remdesivir
![](https://www.drugbank.ca/structures/DB14761/image.svg)

Remdesivir, or GS-5734, is an adenosine triphosphate analog first described in the literature in 2016 as a potential treatment for Ebola.1 In 2017, its activity against the coronavirus family of viruses was also demonstrated.Remdesivir is also being researched as a potential treatment to SARS-CoV2, the coronavirus responsible for COVID-19.
- ## TMC310911
 ![](https://www.drugbank.ca/structures/DB15623/image.svg)

  TMC-310911 (also known as ASC-09) is a novel investigational protease inhibitor (PI) that is structurally similar to the currently available darunavir. It is being investigated for use in HIV-1 infections. TMC-310911 has shown marked activity against a variety of HIV-1 strains, including multi-PI-resistant strains, and may be less likely to generate resistance, making it a potentially desirable therapy for both treatment-naive and PI-experienced patients.

TMC-310911 is currently being investigated, in combination with other HIV therapies and antivirals, as a potential treatment for COVID-19 caused by SARS-CoV-2.
- ## Ritonavir
  ![](https://www.drugbank.ca/structures/DB00503/image.svg)

  Ritonavir is an HIV protease inhibitor that interferes with the reproductive cycle of HIV. Although it was initially developed as an independent antiviral agent, it has been shown to possess advantageous properties in combination regimens with low-dose ritonavir and other protease inhibitors. It is now more commonly used as a booster of other protease inhibitors and is available in both liquid formulation and as capsules.

While ritonavir is not an active antiviral agent against hepatitis C virus (HCV) infection, it is added in combination therapies indicated for treatment of HCV infections as a booster. Ritonavir is a potent CYP3A inhibitor that increases peak and trough plasma drug concentrations of other protease inhibitors such as Paritaprevir and overall drug exposure. American Association for the Study of Liver Diseases (AASLD) and the Infectious Diseases Society of America (IDSA) guidelines recommend ritonavir-boosted combination therapies as a first-line therapy for HCV Genotype 1a/b and 4 treatment-naïve patients with or without cirrhosis.

Ritonavir is found in a fixed-dose combination product with Ombitasvir, Dasabuvir, and Paritaprevir as the FDA-approved product Viekira Pak. First approved in December 2014, Viekira Pak is indicated for the treatment of HCV genotype 1b without cirrhosis or with compensated cirrhosis, and when combined with Ribavirin for the treatment of HCV genotype 1a without cirrhosis or with compensated cirrhosis.

Ritonavir is also available as a fixed-dose combination product with Ombitasvir and Paritaprevir as the FDA- and Health Canada-approved product Technivie. First approved in July 2015, Technivie is indicated in combination with Ribavirin for the treatment of patients with genotype 4 chronic hepatitis C virus (HCV) infection without cirrhosis or with compensated cirrhosis.

In Canada, ritonavir is also available as a fixed-dose combination product with Ombitasvir, Dasabuvir, and Paritaprevir as the Health Canada-approved, commercially available product Holkira Pak. First approved in January 2015, Holkira Pak is indicated for the treatment of HCV genotype 1b with or without cirrhosis, and when combined with Ribavirin for the treatment of HCV genotype 1a with or without cirrhosis. Inclusion of ritonavir can can select for HIV-1 protease inhibitor resistance-associated substitutions. Any HCV/HIV-1 co-infected patients treated with ritonavir-containing combination therapies should also be on a suppressive antiretroviral drug regimen to reduce the risk of HIV-1 protease inhibitor drug resistance.


