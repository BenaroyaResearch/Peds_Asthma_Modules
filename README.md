## Pediatric Asthma Modules

This repository supports the development and use of transcriptome expression modules created as part of the paper
  "A Network of Transcriptome Modules Demonstrates Mechanistic Pathways of Both Viral and Non-viral Induced Asthma Exacerbations in Children"
  
Abstract:

Prevention of asthma exacerbations is an important but unmet medical need as exacerbations cause significant morbidity and health care costs. Although respiratory infections are common precursors to asthma exacerbations in children, the molecular immune responses that determine whether, when and how an infection causes an exacerbation are poorly understood. Using systems-scale network analysis, we identify repertoires of cellular transcriptional pathways that lead to and underlie distinct patterns of asthma exacerbations. Specifically, in both virus associated and non-viral exacerbations, we demonstrate a set of “core” exacerbation modules, consisting of early upregulation of epithelial associated SMAD3 signaling and early down-regulation of lymphocyte response pathways, followed by a later upregulation of effector pathways including epithelial EGFR, extracellular matrix, and mucus hypersecretion, and eosinophil activation. We show an additional set of multiple inflammatory cell pathways involved in virus-associated exacerbations, in contrast to epithelial cell pathways associated with non-viral exacerbations. Through the longitudinal study design, we identify baseline pathways predictive of exacerbation risk, the kinetics of these pathways progressing to a clinical exacerbation, and subsequently which pathways are directly affected by systemic corticosteroid treatment after the onset of an exacerbation. Our work introduces an in vivo molecular platform to investigate, in a clinical setting, both the mechanisms of disease pathogenesis and, importantly, therapeutic targets to modify exacerbations.

### Overview

This repository includes the processed data and code necessary to generate, and apply the modules described in the above paper.  In each of the following sections, we describe how to perform these operations

### Prerequisites

You will need to use [RStudio](https://www.rstudio.com), or possibly [R](https://www.r-project.org) to execute the scripts below that process the data.  The scripts listed below are R-markdown scripts.

### Module Generation

The modules described in the paper came from data collected on two different biological sources, peripherial blood mononuclear cells, and nasal lavage samples.  The processed data necessary for module creation is included in the data directory of this repository.

#### Nasal Modules

To create the nasal modules, "run" the chunks in the file create_nasal_modules_geneSetExpression_Final.Rmd in the modules folder from within RStudio.
The output should be several files in the results directory that assign or associate genes to specific groups, or modules, corresponding to the modules of the paper.

#### Blood Modules

To create the blood modules, "run" the chunks in the file create_blood_modules_geneSetExpression_Final.Rmd in the modules folder from within RStudio.
The output should be several files in the results directory that assign or associate genes to specific groups, or modules, corresponding to the modules of the paper.