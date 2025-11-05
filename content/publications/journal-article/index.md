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
- 
featured: true

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

> [**Section snippets**]

**Introduction**

 Exploratory Data Analysis (EDA) is a comparatively new area of statistics.(Bruce and Bruce, 2017) It is based on the principle that “It is important to understand what you CAN DO before you learn to measure how WELL you seem to have DONE it”(Tukey, 1977). EDA is complementary to confirmatory inferential statistics as it minimises violations of assumptions for model building. It also enables understanding of the data and guides appropriate questions, analysis, and models. Exploratory Spatial Data Analysis (ESDA) is an advancement to EDA for the detection of spatial patterns, hypotheses formulation based on spatial features, and assessing the appropriate spatial models. Similarly, for datasets including both space and time attributes, Exploratory Spatio-Temporal or Space-Time Data Analysis (ESTDA) has been recently introduced and is an active research domain in the field of Geographic Information Science (GIS). (De Smith et al., 2018) The current approach is preferred compared to other methods for time series classification, such as federated distillation learning system (EFDLS)(Xing et al., 2022a), robust temporal feature network (RTFN)(Xiao et al., 2021), and strategies for hybridisation of supervised learning, unsupervised learning, and Self distillation(Xing et al., 2022b). The mathematical foundations for the approach used are underpinned by the fact that dengue counts in routine data have Poison distribution and have been explored to subsequently develop spatiotemporal regression models and time series forecasting for a continuous outcome/ dependent variable. Further, underreporting of mild and missed cases in LMICs and the lack of adequate geocoding accuracy for spatial point pattern analysis pose a limitation for classification algorithms.


**Material and methods**

The present study included secondary data analysis of routinely collected datasets by healthcare system and multiple open-source datasets. The study design was an ecological study in healthcare epidemiology using the data science approach.

**Dengue epidemiology in the state**

The state dengue incidence rates in 2015–19 were 47.8, 33.6, 52.0, 49.7, and 33.4 per 100,000, respectively. The mean (SD) age of the reported dengue cases was 34.3 (16.8) years. Most patients were males (63.9%) and in the age group of 25–39 years (32.0%). The fourth quarter, October, and week 41 to week 46 were dengue's peak periods. The Hurst coefficient of quarterly, monthly, and weekly time series was 0.5, 0.91, and 0.99, and the spectral entropy measure was 0.28, 0.53, and 0.72,

**Discussion**

Dengue occurrence in a population is influenced by ecological and socio-demographic factors (Farrar and Manson, 2014). Exploration of associations between disease occurrence and its eco-socio-demographic factors provides evidence for feature selection and development of early warning forecasting systems for strengthening disease surveillance, efficient resource allocation, and timely implementation of prevention and control measures. The present study is a first-of-kind study from the state

**Conclusion**

The present study provides evidence and a framework for the exploration of Spatio-temporal associations of dengue with ecological and socio-demographic variables in the local context. The study found a high dengue incidence in the state with seasonal patterns. At the sub-district level, changing epidemiology of dengue was observed, which strengthens the call for climate change policy implementation. A non-linear association of dengue with risk factors was seen at multiple lags and with

**Availability of data and algorithms**

All the analyses were carried out using open-domain data sources and reproducible codes, which can be shared with readers on reasonable requests. The data from NVBDCP, Punjab, and Sub-district level spatial files were obtained with restricted use, which can be shared only after additional permissions from the state directorate and Punjab Remote Sensing Authority.




> [!NOTE]
> Click the *Cite* button above to import publication metadata into your reference management software. Further access links for details are arlos provided for your kind perusal and comments.

<!--
> [!NOTE]
> Create your slides in Markdown - click the *Slides* button to check out the example.

Add the publication's **full text** or **supplementary notes** here. You can use rich formatting such as including [code, math, and images](https://docs.hugoblox.com/content/writing-markdown-latex/).

-->
