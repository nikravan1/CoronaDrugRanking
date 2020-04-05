# COVID-19 Drug Ranking


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

The above result shows the Remdesivir and TMC310911 are the best drug for corona virus treatment and chloroquine (Trump had suggested it!) and Triazavirin are the worst.
 - note: These results belong to the best site position which is obtained from SiteMap tools in schrodinger software. you can do these step for any other binding site position or other software.
# How to use it for new drug(Ligand)
 - 1- download 2d or 3d ligand and doing step 1 if needed
 - 2- using proper grid in Grids Folder and doing setp 5 
# Ranking Drug
In this section, all the drugs used to treat covid-19  disease are described (drugbank) in order of their rank.
- ## 1-Remdesivir
![](https://www.drugbank.ca/structures/DB14761/image.svg)

Remdesivir, or GS-5734, is an adenosine triphosphate analog first described in the literature in 2016 as a potential treatment for Ebola.1 In 2017, its activity against the coronavirus family of viruses was also demonstrated.Remdesivir is also being researched as a potential treatment to SARS-CoV2, the coronavirus responsible for COVID-19.
- ## 2-TMC310911
 ![](https://www.drugbank.ca/structures/DB15623/image.svg)

  TMC-310911 (also known as ASC-09) is a novel investigational protease inhibitor (PI) that is structurally similar to the currently available darunavir. It is being investigated for use in HIV-1 infections. TMC-310911 has shown marked activity against a variety of HIV-1 strains, including multi-PI-resistant strains, and may be less likely to generate resistance, making it a potentially desirable therapy for both treatment-naive and PI-experienced patients.

TMC-310911 is currently being investigated, in combination with other HIV therapies and antivirals, as a potential treatment for COVID-19 caused by SARS-CoV-2.
- ## 3-Ritonavir
  ![](https://www.drugbank.ca/structures/DB00503/image.svg)

  Ritonavir is an HIV protease inhibitor that interferes with the reproductive cycle of HIV. Although it was initially developed as an independent antiviral agent, it has been shown to possess advantageous properties in combination regimens with low-dose ritonavir and other protease inhibitors. It is now more commonly used as a booster of other protease inhibitors and is available in both liquid formulation and as capsules.

While ritonavir is not an active antiviral agent against hepatitis C virus (HCV) infection, it is added in combination therapies indicated for treatment of HCV infections as a booster. Ritonavir is a potent CYP3A inhibitor that increases peak and trough plasma drug concentrations of other protease inhibitors such as Paritaprevir and overall drug exposure. American Association for the Study of Liver Diseases (AASLD) and the Infectious Diseases Society of America (IDSA) guidelines recommend ritonavir-boosted combination therapies as a first-line therapy for HCV Genotype 1a/b and 4 treatment-naïve patients with or without cirrhosis.

Ritonavir is found in a fixed-dose combination product with Ombitasvir, Dasabuvir, and Paritaprevir as the FDA-approved product Viekira Pak. First approved in December 2014, Viekira Pak is indicated for the treatment of HCV genotype 1b without cirrhosis or with compensated cirrhosis, and when combined with Ribavirin for the treatment of HCV genotype 1a without cirrhosis or with compensated cirrhosis.

Ritonavir is also available as a fixed-dose combination product with Ombitasvir and Paritaprevir as the FDA- and Health Canada-approved product Technivie. First approved in July 2015, Technivie is indicated in combination with Ribavirin for the treatment of patients with genotype 4 chronic hepatitis C virus (HCV) infection without cirrhosis or with compensated cirrhosis.

In Canada, ritonavir is also available as a fixed-dose combination product with Ombitasvir, Dasabuvir, and Paritaprevir as the Health Canada-approved, commercially available product Holkira Pak. First approved in January 2015, Holkira Pak is indicated for the treatment of HCV genotype 1b with or without cirrhosis, and when combined with Ribavirin for the treatment of HCV genotype 1a with or without cirrhosis. Inclusion of ritonavir can can select for HIV-1 protease inhibitor resistance-associated substitutions. Any HCV/HIV-1 co-infected patients treated with ritonavir-containing combination therapies should also be on a suppressive antiretroviral drug regimen to reduce the risk of HIV-1 protease inhibitor drug resistance.

- ## 4-Galidesivir
  ![](https://www.drugbank.ca/structures/DB11676/image.svg)

  alidesivir is an adenosine analogue that has been investigated for use against Zaire Ebolavirus. In animal studies, galidesivir was effective in increasing the survival rates from infections caused by various pathogens, including Ebola, Marburg, Yellow Fever and Zika viruses. In vitro, it displayed broad-spectrum antiviral activity against various negative- and positive-sense RNA viruses, including coronaviruses, filoviruses, and arenaviruses. Phase 1 clinical trials have begun to determine the safety of this drug in humans. Because of its activity against other coronaviruses, it may be studied as a potential therapy for COVID-19.

- ## 5-Brilacidin
  ![](https://www.drugbank.ca/structures/DB12997/image.svg)

  Brilacidin is under investigation for the supportive care of Mucositis, Stomatitis, Mouth Diseases, and Head and Neck Neoplasms.

- ## 6-Lopinavir
  ![](https://www.drugbank.ca/structures/DB01601/image.svg)

  
Lopinavir is an antiretroviral protease inhibitor used in combination with other antiretrovirals in the treatment of HIV-1 infection.7 Lopinavir is marketed and administered exclusively in combination with ritonavir - this combination, first marketed by Abbott under the brand name Kaletra in 2000, is necessary due to lopinavir's poor oral bioavailability and extensive biotransformation. Ritonavir is a potent inhibitor of the enzymes responsible for lopinavir metabolism, and its co-administration "boosts" lopinavir exposure and improves antiviral activity.7 Like many other protease inhibitors (e.g. saquinavir, nelfinavir), lopinavir is a peptidomimetic molecule - it contains a hydroxyethylene scaffold that mimics the peptide linkage typically targeted by the HIV-1 protease enzyme but which itself cannot be cleaved, thus preventing the activity of the HIV-1 protease.5

Lopinavir is currently under investigation in combination with ritonavir for the treatment of COVID-19 caused by SARS-CoV-2.8

- ## 7-Darunavir
  ![](https://www.drugbank.ca/structures/DB01264/image.svg)

  
Darunavir is a protease inhibitor used with other HIV protease inhibitor drugs as well as ritonavir for the effective management of HIV-1 infection.17 As a second-generation protease inhibitor, darunavir is designed to combat resistance to standard HIV therapy.2,5 It was initially approved by the FDA in 2006.17

Darunavir is being studied as a possible treatment for SARS-CoV-2, the coronavirus responsible for COVID-19, due to in vitro evidence supporting its ability to combat this infection.14 Clinical trials are underway and are expected to conclude in August 2020.19

- ## 8-Nelfinavir
![](https://www.drugbank.ca/structures/DB00220/image.svg)


Nelfinavir is a potent HIV-1 protease inhibitor. It is used in combination with other antiviral drugs in the treatment of HIV in both adults and children. Nelfinavir inhibits the HIV viral proteinase enzyme which prevents cleavage of the gag-pol polyprotein, resulting in noninfectious, immature viral particles.

- ## 9-Atazanavir
  ![](https://www.drugbank.ca/structures/DB01072/image.svg)

  
Atazanavir (formerly known as BMS-232632) is an antiretroviral drug of the protease inhibitor (PI) class. Like other antiretrovirals, it is used to treat infection of human immunodeficiency virus (HIV). Atazanavir is distinguished from other PIs in that it can be given once-daily (rather than requiring multiple doses per day) and has lesser effects on the patient's lipid profile (the amounts of cholesterol and other fatty substances in the blood). Like other protease inhibitors, it is used only in combination with other HIV medications. The U.S. Food and Drug Administration (FDA) approved atazanavir on June 20, 2003.

- ## 10-Favipiravir 
  ![](https://www.drugbank.ca/structures/DB12466/image.svg)

  Discovered by Toyama Chemical Co., Ltd. in Japan, favipiravir is a modified pyrazine analog that was initially approved for therapeutic use in resistant cases of influenza.7,9 The antiviral targets RNA-dependent RNA polymerase (RdRp) enzymes, which are necessary for the transcription and replication of viral genomes.7,12,13

Not only does favipiravir inhibit replication of influenza A and B, but the drug shows promise in the treatment of influenza strains that are resistant to neuramidase inhibitors, as well as avian influenza.9,19 Favipiravir has been investigated for the treatment of life-threatening pathogens such as Ebola virus, Lassa virus, and now COVID-19.

- ## 11-Umifenovir
  ![](https://www.drugbank.ca/structures/DB13609/image.svg)

  Umifenovir is an indole-based, hydrophobic, dual-acting direct antiviral/host-targeting agent used for the treatment and prophylaxis of influenza and other respiratory infections.13 It has been in use in Russia for approximately 25 years and in China since 2006. Its invention is credited to a collaboration between Russian scientists from several research institutes 40-50 years ago, and reports of its chemical synthesis date back to 1993.13 Umifenovir's ability to exert antiviral effects through multiple pathways has resulted in considerable investigation into its use for a variety of enveloped and non-enveloped RNA and DNA viruses, including Flavivirus,2 Zika virus,3 foot-and-mouth disease,4 Lassa virus,6 Ebola virus,6 herpes simplex,8, hepatitis B and C viruses, chikungunya virus, reovirus, Hantaan virus, and coxsackie virus B5.13,9 This dual activity may also confer additional protection against viral resistance, as the development of resistance to umifenovir does not appear to be significant.13

Umifenovir is currently being investigated as a potential treatment and prophylactic agent for COVID-19 caused by SARS-CoV2 infections in combination with both currently available and investigational HIV therapies.

- ## 12-Chloroquine
  ![](https://www.drugbank.ca/structures/DB00608/image.svg)

  Chloroquine is an aminoquinolone derivative first developed in the 1940s for the treatment of malaria.4 It was the drug of choice to treat malaria until the development of newer antimalarials such as pyrimethamine, artemisinin, and mefloquine.17 Chloroquine and its derivative hydroxychloroquine have since been repurposed for the treatment of a number of other conditions including HIV, systemic lupus erythematosus, and rheumatoid arthritis.18

Chloroquine was granted FDA Approval on 31 October 1949.20

Due to COVID-19, the FDA has issued an emergency use authorization for hydroxychloroquine and chloroquine.22 This authorization allows for the unapproved use of these medications in light of a public health emergency.

- ## 13-Triazavirin
  ![](https://www.drugbank.ca/structures/DB15622/image.svg)


Triazavirin is a guanine nucleotide analog antiviral originally developed in Russia that has shown efficacy against influenza A and B, including the H5N1 strain.1,2,4 It appears that Triazavirin has shown promise in reducing influenza disease severity and associated complications.5 Given the similarities between SARS-CoV-2 and H5N1, health officials are investigating Triazavirin as an option to combat SARS-CoV-2, the coronavirus responsible for COVID-19.

