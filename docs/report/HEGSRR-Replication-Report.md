---
layout: page
title: RE- Replication of Rosgen Stream Classification
---


**Replication of**
# A classification of natural rivers

Original study *by* Rosgen, D. L.
*in* *CATENA* 22 (3):169–199. https://linkinghub.elsevier.com/retrieve/pii/0341816294900019.

and Replication by: Kasprak, A., N. Hough-Snee, T. Beechie, N. Bouwes, G. Brierley, R. Camp, K. Fryirs, H. Imaki, M. Jensen, G. O’Brien, D. Rosgen, and J. Wheaton. 2016. The Blurred Line between Form and Process: A Comparison of Stream Channel Classification Frameworks ed. J. A. Jones. *PLOS ONE* 11 (3):e0150293. https://dx.plos.org/10.1371/journal.pone.0150293.

Replication Authors:
Jacob Freedman, Zach Hilgendorf, Joseph Holler, and Peter Kedron.

Replication Materials Available at: [Re-Rosgen](https://github.com/jafreedman12/RE-rosgen)

Created: `19 March 2021`
Revised: `19 March 2021`


## Abstract

In this study, we are replicating Rosgen's (1994) seminal classification of river systems, an effort that was originally undertaken to make the understanding of rivers transferable across disciplines. By looking at the surrounding landscape and the composition of the river, Rosgen (1994) hypothesized that a river classification system could be created and replicated for use in multiple disciplines. While previous studies attempted to classify streams based on age (Davis 1899), slope (Schumm 1963), bedload (Schumm 1977), valley pattern (Thornbury 1969), and pattern of movement (Brice and Blodgett 1978), among with many others, each of these was not effective for classifying streams across a variety of landscapes. By combining elements from all of these previous classifications, Rosgen focused on sinuosity, entrenchment, and widths of flood-prone areas to construct a multi-level classification system that emphasized the hierarchies of "states" of a river. Building on this research, Kasprak et al. (2016) set out to examine the replicability and accuracy of the Rosgen classification system (along with other classification systems), using spatial analysis tools at a watershed scale. Looking at the Middle Fork of the John Day River watershed, Kasprak et al. (2016) used DEM data and field-collected river data

In this analysis, we are working to replicate the Rosgen classification system as replicated by Kasprak et al. (2016), all while using open-source GIS resources. By testing this replicability, we

## Original Study Information

While Rosgen (1994) provides a framework for the Rosgen Classification System at various levels (relevant here are Level I: general landscape form, and Level II: more specific, field-based measurements), the research by Kasprak et al. (2016) provides an opportunity for us to replicate an existing automation of a framework. One of the major challenges with river classification is the variability between classification systems and the need for data gathered in the field. While both our analysis and that by Kasprak et al. (2016) use information from the field about stream bed composition, the capacity to do a large portion of these analyses using aerial imagery and GIS reflects immense possibilities in the easier replication and comparison of river classification systems.

For the purposes of this report, I will focus on the use of the Rosgen Classification System (RCS) by Kasprak et al. (2016), although they compared this analysis with the River Styles Framework, the Columbia Basin Natural Channel Classification, and a Statistical Classification. Kasprak et al. (2016) set out to classify rivers at the watershed scale, using the Middle Fork of the John Day River Watershed (MFJD) as a test location. With an immense amount of field data collected for this site because of salmon monitoring, it was possible to complete the RCS and the other classifications without needing to collect river samples on their own. Using 33 points of analysis from the CHaMP (Columbia Habitat Monitoring Program) dataset, Kasprak et al. (2016) used 10m and 0.1m DEMs 1m aerial imagery to determine the Level I classifications at each CHaMP point. Level II classifications of width-depth ration, sinuosity, entrenchment, and gradient were calculated from O.1m DEMs and the River Bathymetry Toolkit.

The data from this original analysis can be found in our publically-available ["Re-Rosgen"] (https://github.com/jafreedman12/RE-rosgen)repository. [CHaMP shapefiles] (https://github.com/jafreedman12/RE-rosgen/tree/main/data/raw/public) and [DEM data for the John Day Watershed] (https://github.com/jafreedman12/RE-rosgen/tree/main/data/raw/private) can be found at the corresponding links.

## Analytical Plan

Describe all elements of the analytical plan of the original study that are relevant to the research questions and hypotheses being re-examined by the replication. Include information for each of the following sub-sections as appropriate.

### Sampling Plan and Data Description

In our class of 18 students, we were each [randomly assigned](https://gis4dev.github.io/lessons/04b_rosgen_GRASS_R.html) a study site for this analysis. I was assigned Location 13, seen below in Figure 1.

 Figure 1: Point of analysis (Location 13) in the CHaMP dataset in the MFJD watershed
 ![Image of Locator Map, showing Point 13 (orange) in MFJD watershed](https://octodex.github.com/images/yaktocat.png)



Describe the data used in the original study. If sampling was used, provide details about the sampling design and how it was implemented.
1. Describe how sampled data relevant to the hypotheses being re-examined was collected by the original authors.
   -	For human subjects research, include the population from which subjects were sampled, location of sampling, recruitment details, payments for participation, eligibility criteria (e.g. inclusion and exclusion rules), and sampling timeline.
   -	For research that did not involve human subjects, include information about sample collection, duration of data gathering efforts, source or location of samples
   -	For studies in which sample location is obfuscated, explain the motivation for the obfuscation and identify the type of geographic masking technique that was used.  
2. Describe the spatial sampling design used during data collection
   -	Identify the design of the spatial sample (e.g., stratified random sample)
   -	Identify the size of the sample, and how many observations will be collected in different geographic strata or levels if using a stratified, clustered, or multilevel design.
   -	If a termination rule was used, identify the relevant criteria, original authors’ motivation, and how the rule was implemented.
3. Describe any secondary dataset(s), or sub-set(s) of those datasets, used in the original study.
   -	Explain how the data was acquired by the original authors including – source (with DOI if possible), data of access
   -	If selected datasets or sub-sets cover only portions of the overall study area or study period, clearly identify which datasets are associated with which locations and times.
   -	Explain how the data was acquired by the original authors including – source, data of access
4. Describe if/how the original study excluded or adjusted the initial dataset
   -	Identify any data that was excluded from the original analysis report –reason for exclusion, exclusion criteria, sample size before and after exclusion, location of excluded data (e.g., is exclusion likely to reduce/eliminate coverage in a particular sub-region)
   -	Explain how the original authors addressed missing data and details about any interpolation procedures used by the authors.
   -	Describe any sample weighting that was used in the original study. Separately identify any spatial component used in the weighting scheme.

### Variables

Describe the variables used in the original study to address the research questions and hypotheses that are the focus of the replication.

1. Identify any experimentally manipulated variables and include details about how these variables were manipulated during the original study.
2. Identify any measured variables examined in the original study
   -	Identify both the response(s) and predictor variable(s) associated with each hypothesis
   -	Describe any variable transformations (e.g., log-scaled, categorical)
   -	Describe any spatial aggregation/disaggregation that was applied to any variables
3. Describe any adjustments made to the variables to account for
   -	first-order spatial effects (sub-regional differences in means)
   -	second-order spatial effects (spatial dependencies)
   -	spatial anisotropies (directional trends)

### Analytical Specification

Describe the exact analytical specification that was used to test each hypothesis
1. For computational studies include information about the hardware and software environments of both the original study
2. Identify the coordinate system(s) and projection(s) used during the original analysis
3. Specify if/how edge effects were addressed. Provide details regarding the extent of any buffer or guard areas used.
4. Describe the type of model, the specification of that model, distributional assumptions of the model, and any post-hoc analyses used to test each hypothesis. Key aspects of some common geographical analyses include:
   - If a spatial weighting scheme was used, provide a functional description of that scheme
   - If a spatial model was used, provide detailed description of that model
   - If a classifier was used, provide details about the selection of training data, validation data, and if any independent test data
   - If a spatial multi-level model was used, identify the spatial scale of each level, the variable included at each level, and the levels any spatial structures or cross-scale structure are estimated at.
Inference Criteria, Results, and Robustness: For each separate hypothesis, provide a description of the results of the original study and the relevant inference criteria and robustness checks
1. Describe the specific criteria (e.g., p-values, effect size, model fit) and thresholds that were used to make inferences.
   -	Identify any adjustments made for multiple testing (e.g., Bonferroni, Sidak) and how they were implemented.
2. Describe the result associated with each hypothesis.
   -	Identify the size and direction of the effect, measure of variance of the effect, statistical assessments
3. Describe any robustness checks that were completed to assess the strength and reliability of inferences for each hypothesis. Identify any spatial components varied during robustness checks.

## Materials and Procedure

Describe how the replication study will be implemented and identify any materials and procedures used to complete the replication.
1.	For computational studies include information about the hardware and software environments of both the original study and the replication attempt.

Protocol: Explain how the analysis of the replication will proceed and identify if the analysis plan will match the original study. For many replications this section may be quite short if the procedures used in the original analyses are followed closely. In those cases, this section can simply explain how key elements will be followed.

Differences from the Original Study: Identify any ways in which the replication is planned to depart from the original study -- a) location, b) sampling, c) data, d) measures/variable construction, d) analytical techniques.
1.	Provide the motivation for each change that is made to the original study.
2.	State how the differences identified above may influence the expected size/direction of the effect of the original study
3.	List any testable hypotheses associated with each change. If a hypothesis is directional, state the direction
4.	Outline any initial analyses that were taken to assess whether the differences identified above will influence the outcome of the replication attempt.

Assessment Criteria: Identify the criteria that will define whether the replication attempt was successful (e.g., matched statistical significance, direction of effect, similar magnitude of effect)
- Reproducible documentation of methods, where documentation includes:
- Annotated flowchart of final parameter values (use last page of RSC_EPA_2005 PDF)

## Replication Results

For each hypothesis examined, present separately the results of the replication attempt.
1.	Briefly describe how the replication protocol outlined above was implemented reporting key information (e.g., sample size).
2.	State whether the original hypothesis was or was not supported by the replication
   - Provide key statistics produced by the replication.
   - Provide key measures (e.g., matching effect direction/size, significance) used to make the decision.
   - Highlight any contradictory results with a brief explanation
3.	State whether any hypothesis linked to a planned deviation from the original study was supported. Provide key statistics and related reasoning.

Figures to Include:
- map of the study site shaded elevation
- map of the study site slope
- Map of the study site stream/river centerlines and final mean centerline
- Map of the study site valley centerlines and final mean centerline
- Longitudinal profile graph with elevation and slope
- Cross-sectional profile graph

Tables to Include:

Table 1. Site Measurements
| Variable | Value | Source |
| :-: | :-: | :-: |
| Bankfull Width (m) | 8.0755 |  [CHaMP_Data_MFJD](https://github.com/jafreedman12/RE-rosgen/tree/main/data/raw/public)|
| Bankfull Depth Average (m) | 0.4031 | [DpthBf_Avg in  CHaMP_Data_MFJD](https://github.com/jafreedman12/RE-rosgen/tree/main/data/raw/public) |
| Bankfull Depth Maximum (m) | 1.7449 | [DpthBf_Max in CHaMP_Data_MFJD](https://github.com/jafreedman12/RE-rosgen/tree/main/data/raw/public) |
| Valley Width (m) | 325 | *last graph in rstudio code |
| Valley Depth (m) | 3.4998 | *calculation of MaxBFx2|
| Stream/River Length (m) | 306.66 | *calculation in grass |
| Valley Length (m) | 230.17 | *calculation in grass |
| Median Channel Material Particle Diameter (mm) | 70 | [SubD50 variable in CHaMP_Data_MFJD](https://github.com/jafreedman12/RE-rosgen/tree/main/data/raw/public) |

Table 2. Rosgen Level I Classification
| Criteria | Value |
| :-: | :-: |
| Entrenchment Ratio | -- |
| Width / Depth Ratio | -- |
| Sinuosity | -- |
| Level I Stream Type | -- |

Table 3. Rosgen Level II Classification
| Criteria | Value |
| :-: | :-: |
| Slope | -- |
| Channel Material | -- |
| Level II Stream Type | -- |


## Unplanned Deviations from the Protocol

Identify and describe any unplanned deviations from the original replication protocol the occurred during the course of the replication. Explain the rationale behind any deviations. Finally, provide the details and results of any sensitivity analyses conducted to assess whether these deviations may have impacted the results of the replication.

## Discussion

Provide a summary and interpretation of the key findings of the replication *vis-a-vis* the original study results. If the attempt was a failure, discuss possible causes of the failure. These may include:
- Practical Causes – related to lack of data, code, details in the original analysis
- Informative Causes – related to absence of effect, change in population, or location.

Discuss an interpretation of your results.
- Were the Level I and Level II results internally and logically consistent? That is, did all the parameters for the identified stream type conform to expectations outlined in Rosgen?
- Were your results consistent with previous evaluations of the same stream reach reported by Kasperak et al?

Discuss a response to the following prompt: Quantifying uncertainty in geomorphic systems and in GIScience is of paramount importance, not only for creating error bars on a graph, but for realistically communicating the reliability and legitimacy of an output dataset. Error bars do not (necessarily) reflect on the researcher. They stem from collection constraints, processing constraints, subjective decision making, and many, many more sources. Given what you have learned in this module, discuss at least three sources of error and uncertainty and how they could impact the classification of your stream. Where does uncertainty stem from? Why is uncertainty a problem? What could be done (or has been done) to fix or reduce uncertainty? In a perfect world, how could this uncertainty be removed?

## Conclusion

Restate the key findings and discuss their broader societal implications or contributions to theory.
Do the research findings suggest a need for any future research?

## References

Include any referenced studies or materials in the [AAG Style of author-date referencing](https://www.tandf.co.uk//journals/authors/style/reference/tf_USChicagoB.pdf).

####  Report Template References & License

This template was developed by Peter Kedron and Joseph Holler with funding support from HEGS-2049837. This template is an adaptation of the ReScience Article Template Developed by N.P Rougier, released under a GPL version 3 license and available here: https://github.com/ReScience/template. Copyright © Nicolas Rougier and coauthors. It also draws inspiration from the pre-registration protocol of the Open Science Framework and the replication studies of Camerer et al. (2016, 2018). See https://osf.io/pfdyw/ and https://osf.io/bzm54/

Camerer, C. F., A. Dreber, E. Forsell, T.-H. Ho, J. Huber, M. Johannesson, M. Kirchler, J. Almenberg, A. Altmejd, T. Chan, E. Heikensten, F. Holzmeister, T. Imai, S. Isaksson, G. Nave, T. Pfeiffer, M. Razen, and H. Wu. 2016. Evaluating replicability of laboratory experiments in economics. Science 351 (6280):1433–1436. https://www.sciencemag.org/lookup/doi/10.1126/science.aaf0918.

Camerer, C. F., A. Dreber, F. Holzmeister, T.-H. Ho, J. Huber, M. Johannesson, M. Kirchler, G. Nave, B. A. Nosek, T. Pfeiffer, A. Altmejd, N. Buttrick, T. Chan, Y. Chen, E. Forsell, A. Gampa, E. Heikensten, L. Hummer, T. Imai, S. Isaksson, D. Manfredi, J. Rose, E.-J. Wagenmakers, and H. Wu. 2018. Evaluating the replicability of social science experiments in Nature and Science between 2010 and 2015. Nature Human Behaviour 2 (9):637–644. http://www.nature.com/articles/s41562-018-0399-z.
