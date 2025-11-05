---
title: "Exploratory Spatio-Temporal Data Analysis (ESTDA) of Dengue and its association with climatic, environmental, and sociodemographic factors in Punjab, India"
authors:
- admin
- Dr Biju Soman
- Dr Gagandeep Singh Grover
date: "2023-07-01"

# Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "*Ecological Informatics*"
publication_short: ""

abstract: Routine health data is rich in information but underutilised for research in Low and Middle-Income countries. The present study was carried out to understand spatiotemporal patterns of dengue and its association with risk factors using routine data from health and allied sectors. ESTDA included estimation of dengue incidence rates, time series features and correlation coefficients up to the sub-district level. Scatter plots and correlation coefficients were used to identify relationships between covariates. Dengue incidence in 2015–19 was 47.76, 33.64, 52.03, 49.71, and 33.36 per 100,000, respectively, with a mean (SD) age of 34.33 (16.78) years and the majority being males (63.94%). Dengue had significant cross-correlation, non-linear relationships, and spatio-temporal associations with climatic, environmental, and socio-demographic risk factors. Significant autocorrelation of dengue occurrence was present at a lag of one month with seasonal patterns. The reproducible open-source algorithms add value to existing Routine Health Information Systems, and the findings will enable the development of Spatio-temporal models in future research. The research was done using R version 4.1.0.

summary: The study was carried out to understand spatiotemporal patterns of dengue and its association with risk factors using routine data from health and allied sectors using Data Science open-source methods.

tags:
- Source Themes
featured: false

#hugoblox:
 # ids:
  #  arxiv: 1512.04133v1

links:
  - type: pdf
    url: https://www.researchgate.net/publication/368432733_Exploratory_Spatio-Temporal_Data_Analysis_ESTDA_of_Dengue_and_its_association_with_climatic_environmental_and_sociodemographic_factors_in_Punjab_India
  # - type: code
   #  url: https://github.com/HugoBlox/hugo-blox-builder
  # - type: dataset
    # url: ""
  # - type: poster
    # url: ""
  # - type: project
    # url: ""
  # - type: slides
    # url: https://www.slideshare.net/
  - type: source
    url: https://www.researchgate.net/publication/368432733_Exploratory_Spatio-Temporal_Data_Analysis_ESTDA_of_Dengue_and_its_association_with_climatic_environmental_and_sociodemographic_factors_in_Punjab_India
  # - type: video
    # url: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: "**Ecological Informatics**"
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: [data-visualization]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---


Introduction
“Systems that comprise data collected at regular intervals at public, private, and community-level health facilities and institutions and health programs” are Routine Health Information Systems (RHIS).(MEASURE Evaluation, 2022) RHIS systematically collects data, often for administrative use within health departments. Despite being rich in information, RHIS is underutilised for research in low- and middle-income countries, especially in the Asian subcontinent.(Hung et al., 2020).
The use of interdisciplinary approaches by linking data from non-health sectors and GIS is recommended by WHO-India Joint Monitoring Mission to strengthen disease surveillance.(Directorate General of Health Services, India, 2015) Data science is “an interdisciplinary field involving processes, theories, concepts, tools, and technologies, that enable the review, analysis, and extraction of valuable knowledge and information from structured and unstructured (raw) data.(Data Science - MeSH - NCBI, 2023) Thus, data science allows researchers to explore and analyse routine health data and its associations with ecological datasets.(van der Aalst, 2016).
Dengue is the fastest growing Vector Borne Disease (VBD) globally, and the highest burden is present in Low- and Middle- Income Countries (LMICs). South-East Asian Region (SEAR) contributes to 52% of the global dengue burden and is a significant public health problem in India. Dengue incidence in a population is determined by climatic, environmental, and socio-demographic conditions. These associations vary from place to place, and it is essential to understand them in the local context to develop Spatio-temporal models for evidence-informed public health decision-making.
Exploratory Data Analysis (EDA) is a comparatively new area of statistics.(Bruce and Bruce, 2017) It is based on the principle that “It is important to understand what you CAN DO before you learn to measure how WELL you seem to have DONE it”(Tukey, 1977). EDA is complementary to confirmatory inferential statistics as it minimises violations of assumptions for model building. It also enables understanding of the data and guides appropriate questions, analysis, and models. Exploratory Spatial Data Analysis (ESDA) is an advancement to EDA for the detection of spatial patterns, hypotheses formulation based on spatial features, and assessing the appropriate spatial models. Similarly, for datasets including both space and time attributes, Exploratory Spatio-Temporal or Space-Time Data Analysis (ESTDA) has been recently introduced and is an active research domain in the field of Geographic Information Science (GIS). (De Smith et al., 2018) The current approach is preferred compared to other methods for time series classification, such as federated distillation learning system (EFDLS)(Xing et al., 2022a), robust temporal feature network (RTFN)(Xiao et al., 2021), and strategies for hybridisation of supervised learning, unsupervised learning, and Self distillation(Xing et al., 2022b). The mathematical foundations for the approach used are underpinned by the fact that dengue counts in routine data have Poison distribution and have been explored to subsequently develop spatiotemporal regression models and time series forecasting for a continuous outcome/ dependent variable. Further, underreporting of mild and missed cases in LMICs and the lack of adequate geocoding accuracy for spatial point pattern analysis pose a limitation for classification algorithms.
Increasing initiatives for improving RHIS data quality in LMICs have been undertaken in the past few decades; however, neglected tropical diseases such as dengue require additional efforts to understand the data structure, quality issues, and mechanisms by which evidence can be generated from the routinely collected data.
India contributes to around 34% of the global burden of dengue.(Dengue and severe dengue, 2023) However, the association of dengue with risk factors in the country is poorly explored. Also, because of multiple climatic zones and varied ecology and socio-demography within the states in India, the exploration of such associations in local context is recommended.(Kakarla et al., 2019) Further, in the majority of studies carried out in the country on dengue and its risk factors using RHIS, the association of dengue has been explored for associations with either a single risk factor, or at a spatial granularity of national or state level or with isolated spatial or time series analysis. There is an unmet need for studies exploring dengue association with multiple climatic, environmental, and socio-demographic factors at higher resolution for understanding disease dynamics. There is an evident lack of studies to understand dengue epidemiology using satellite imagery datasets, its space-time associations with multiple risk factors, and the use of advancements in technology which can provide decision support to public health managers. There is also a dearth of open-source solutions to foster research using RHIS. Additionally, within the health sector, on the one hand, there are robust RHIS such as Nickshay for Tuberculosis, digitisation for Reproductive and Maternal Health, etc., on the other, routine data for Dengue occurrence still exists in excel sheets is entered manually, and poses challenges to its use in research. Therefore, the present study was thus undertaken as ESTDA in data science using dengue routine health data and open-source software to explore patterns and associations for dengue incidence and its climatic, environmental, and socio-demographic risk factors in Punjab, India.



> [!NOTE]
> Click the *Cite* button above to import publication metadata into your reference management software. Further access links for details are arlos provided for your kind perusal and comments.

<!--
> [!NOTE]
> Create your slides in Markdown - click the *Slides* button to check out the example.

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).

-->
