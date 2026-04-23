# Aligning Behavioural Ecotoxicology with Real-World Water Concentrations: Current Minimum Tested Levels for Pharmaceuticals Far Exceed Environmental Reality

This repository contains all the scripts for the comparative analysis of pharmaceutical concentrations used in **laboratory-based exposure experiments** versus those detected in **natural field environments** in Martin et al (2025).

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). You are free to reuse, redistribute, and adapt the material, provided appropriate credit is given.

------------------------------------------------------------------------

## 📖 Project Overview

Pharmaceutical pollution is an escalating issue, with widespread contamination now well-documented across aquatic ecosystems globally. In parallel, research into the behavioural effects of pharmaceuticals on aquatic organisms has expanded rapidly, revealing that some of these compounds can alter behaviour even at environmentally relevant concentrations. However, a recent systematic evidence map on this topic has highlighted substantial variability in the exposure concentrations used across behavioural tests---raising questions about their environmental realism. In this study, we compare 767 behavioural assays with over 10 million pharmaceutical occurrence records from three major global monitoring databases. Our analysis reveals that minimum tested concentrations in behavioural studies are, on average, 43 times higher than median surface water concentrations and 10 times higher than median concentrations in treated wastewater. Notably, more than half of the tested compounds were never assessed at levels below the 95% credible interval of observed wastewater concentrations. Furthermore, the pharmaceuticals most frequently tested in behavioural assays showed only weak correspondence with those most commonly detected in the environment. These findings suggest a significant misalignment between experimental design and environmental reality, potentially limiting the relevance of behavioural ecotoxicology for ecological risk assessments and evidence-based environmental regulation.

------------------------------------------------------------------------

## 📝 Associated article

-   **Title**: *Aligning Behavioural Ecotoxicology with Real-World Water Concentrations: Current Minimum Tested Levels for Pharmaceuticals Far Exceed Environmental Reality*\

-   **Authors**: Jake M. Martin^1,2,3,📩^, Jack A. Brand^2,4^, Erin S. McCallum^2^\

-   **Institutions**:\
    1 School of Life and Environmental Sciences, Deakin University, Geelong, Victoria, Australia\
    2 Department of Wildlife, Fish, and Environmental Studies, Swedish University of Agricultural Sciences, Umeå, Sweden\
    3 School of Biological Sciences, Monash University, Clayton, Victoria, Australia\
    4 Institute of Zoology, Zoological Society of London, London, United Kingdom\
    📩 Corresponding author\

-   **Status**: Published.  *Environ. Sci. Technol. Lett. 2025, 12, 10, 1308–1313.* https://doi.org/10.1021/acs.estlett.5c00665

------------------------------------------------------------------------

## 📁 Repository Structure

```         
📂 field-vs-lab-doses/
├── 📂 fig/                                     # All figures associated with the project
├── 📂 mods/                                    # All statistical models associated with the project
├── 📄 field-vs-lab-doses-1.Rmd                 # R script used to tidy and combind all the databases 
├── 📄 field-vs-lab-doses-2.Rmd                 # R script used for data analysis and visualisation
├── 📄 field-vs-lab-doses-3.Rmd                 # R script used for QA/QC sub-set sensitivity analysis
├── 📄 martin-et-al-supplementary-file-2...html # Summary table for environmental occurrence
└── 📄 index.html                               # A htlm knit of 'field-vs-lab-doses-2.Rmd' used as a git hub page
```

------------------------------------------------------------------------

## 📥 How to Use

1.  **Clone the repository:**

    ``` bash
    git clone https://github.com/JakeMartinResearch/field-vs-lab-doses.git
    ```

2.  **Download data** you can download data from OSF framework and save in called data within the project directory. Martin, J. M., Brand, J. A., & McCallum, E. (2025). Aligning Behavioural Ecotoxicology with Real-World Water Concentrations. <https://doi.org/10.17605/OSF.IO/H6CDE>

-   [`EIPAAB-database.csv`](https://osf.io/uvnht/download)

-   [`pharms-uba_v3_2021_0.xlsx`](https://osf.io/6a7vd/download)

-   [`pnas.2113947119.sd04.xlsx`](https://osf.io/gp5tw/download)

-   [`norman_pharma.csv`](https://osf.io/g6h37/download)

-   [`pubchem-compound-identifiers.csv`](https://osf.io/pqnbx/download)

-   [`martin-field-vs-lab-all-databases.csv`](https://osf.io/ht6sk/download)/

    For example.../

    ```         
    📂 field-vs-lab-doses/
     └── 📂 data/  
          ├── 📄 EIPAAB-database.csv
          ├── 📄 pharms-uba_v3_2021_0.xlsx
          ├── 📄 pnas.2113947119.sd04.xlsx
          ├── 📄 norman_pharma.csv
          ├── 📄 pubchem-compound-identifiers.csv
          └── 📄 martin-field-vs-lab-all-databases.csv
    ```

3.  **Run scripts** from the `scripts/` directory in any order:

    -   `field-vs-lab-doses-1.Rmd`
    -   `field-vs-lab-doses-2.Rmd`
    -   `field-vs-lab-doses-3.Rmd`

------------------------------------------------------------------------

## 📜 Download or Pull This Repository into R

To work with this project in RStudio:

1.  Open RStudio → **File** → **New Project** → **Version Control** → **Git**

2.  Paste this URL in the **Repository URL** field:

```{=html}
https://github.com/JakeMartinResearch/field-vs-lab-doses.git
```
3.  Choose a folder on your computer

4.  Click **Create Project**

RStudio will now pull the GitHub repo into a new local folder.

📺 [Watch this 2-min tutorial on YouTube](https://www.youtube.com/watch?v=HzTqHk4XjQQ)

------------------------------------------------------------------------

## 📊 Outputs

-   HTML-rendered results and figures are available at:\
    📍 <https://jakemartinresearch.github.io/field-vs-lab-doses/>

-   Bayesian model outputs are saved as `.rds` files and stored in the `/mod/` folder.

------------------------------------------------------------------------

## 📑 Citation

If you use or adapt the methods used in this repository, please cite:

> Martin JM. Brand JA, McCallum ES. Aligning Behavioural Ecotoxicology with Real-World Water Concentrations: Current Minimum Tested Levels for Pharmaceuticals Far Exceed Environmental Reality. *Environ. Sci. Technol. Lett.*, 2025;12,10:1308–1313. DOI: 10.1021/acs.estlett.5c00665

If you use the collated database `martin-field-vs-lab-all-databases.csv`, please also cite:

> Wilkinson JL, Boxall ABA, Kolpin DW, Leung KMY, Lai RWS, Wong D, et al. Pharmaceutical pollution of the world’s rivers. *Proc. Natl. Acad. Sci. USA*. 2022;119:1–10. DOI: 10.1073/pnas.2113947119.

> Network N. NORMAN EMPODAT Database - Chemical Occurrence Data [Internet]. Available from: https://www.norman-network.com/nds/empodat

> aus der Beek T, Weber FA, Bergmann A, Hickmann S, Ebert I, Hein A, et al. Pharmaceuticals in the environment-Global occurrences and perspectives. *Environ Toxicol Chem*. 2016;35:823–35.DOI:10.1002/etc.3339.  

------------------------------------------------------------------------

## 📩 Contact

**Jake M. Martin**

📧 **Email:** [jake.martin\@deakin.edu.au](mailto:jake.martin@deakin.edu.au)

📧 **Alt Email:** [jake.martin.research\@gmail.com](mailto:jake.martin.research@gmail.com)

🌐 **Web:** [jakemartin.org](https://jakemartin.org/)

🧪 **ORCID**: [0000-0001-9544-9094](https://orcid.org/0000-0001-9544-9094)

------------------------------------------------------------------------
