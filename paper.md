title: 'FANGS - Fire Applications with Next Generation Satellites'
tags:
  - python
  - jupyter notebooks
  - copernicus
  - atmospheric composition
  - wildfires
  - open data
authors:

  - name: Sabrina H. Szeto
    orcid: 0000-0002-3050-837X
    affiliation: 1
  - name: Julia Wagemann
    orcid: 0000-0002-3075-2559
    affiliation: 2
  - name: Simone Mantovani
    orcid: 0000-0003-3979-3645
    affiliation: 3
  - name: Federico Fierli
    orcid: 0000-0001-9975-2883
    affiliation: 4
affiliations:
 - name: Sabrina Szeto Consulting
   index: 1
 - name: Julia Wagemann Consulting
   index: 2
 - name: Meteorological Environmental Earth Observation (MEEO) s.r.l.
   index: 3
 - name: European Organisation for the Exploitation of Meteorological Satellites (EUMETSAT)
   index: 4
date: 30 December 2022
bibliography: paper.bib
---

# Summary

The FANGS training course consists of Python-based training material and application examples on detection and monitoring of the fire life-cycle. It is developed by the European Organisation for the Exploitation of Meteorological Satellites (EUMETSAT). The developed training material makes use of proxy and simulated data, including data from precursor instruments of the Meteosat Third Generation (MTG) and the EUMETSAT Polar System - Second Generation (EPS-SG) / Metop Second Generation (Metop-SG) satellite missions. The training material is developed in the form of modular Jupyter notebook case studies on the 2020 wildfires in California, USA and the Mediterranean wildfires in 2021. In total, 24 notebooks were developed comprising five narrative notebooks and 19 workflow notebooks. These notebooks are available on a [Gitlab repository](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring) as well as on a dedicated [FANGS JupyerLab platform](https://fire.adamplatform.eu), where the notebooks can be executed. In addition, an accompanying [Jupyter Book](https://firebook.ltpy.adamplatform.eu/) is also available as an entrypoint to the material.

# Statement of Need

As climate models predict a growing intensity and frequency of wildfire events in the future [@ipcc], Earth Observation (EO) data from satellites are an increasingly valuable source of information for wildfire monitoring, particularly for regions with a Mediterranean climate which are particularly susceptible to fires [@turco]. In the near future, new instruments aboard satellites from the MTG and Metop-SG missions will provide advanced capabilities and valuable data for monitoring wildfires and their impacts. Data users, for example researchers, emergency management agencies and land managers among others, need to gain familiarity with the upcoming data as well as their improved capabilities. While data from these instruments are not yet available, proxy data from existing and precursor instruments as well as simulated data can be used for training and preparing new data users. Proxy data refers to “data with valid scientific content, to be used in early training on instrument capabilities and application areas, for example in test beds. These are real datasets from relevant existing precursor instruments [@eumetsat].”

In order to familiarise more data users with the upcoming datasets, we developed a modular set of training materials for data users to learn about the applications of the upcoming data from the MTG and Metop-SG satellite missions. 

# Learning Objectives and Instructional Design

There are two main learning objectives of the FANGS training course. Firstly, the training course introduces data users to upcoming instruments aboard the MTG and Metop-SG satellites which are useful for monitoring wildfires. Secondly, it provides step-by-step workflows and examples for loading, processing and visualising proxy data and other associated datasets in the context of actual wildfire events, namely the Mediterranean wildfires in 2021 and the wildfires in California, USA in 2020.

Each case study consists of two to six narrative notebooks describing the wildfire event and how the upcoming MTG and EPS-SG satellites will improve the capabilities to monitor the full fire life cycle, together with figures comprising maps and animations of satellite data products for each event. The narrative notebooks highlight different parts of the fire life cycle - from pre-fire risk, active burning and smoke transport to assessing post-fire impacts. Each figure in the narrative notebooks is linked to a workflow notebook showing how the proxy data from MTG and EPS-SG were loaded, processed and visualised.

In order to cater to data users with different levels of Python experience, we use several predefined functions that enable data users to load, pre-process and visualise data easily [@wagemann]. For those who are new to Python, this enables them to apply the functions directly by adding the required keyword arguments. For those with more advanced knowledge, they can open the functions notebook and modify the functions even further. 

The training course has been developed to enable data users to dive as deep as they want into the material. For data users who just want to read through the case studies and look at the example figures, they can access them through a [Jupyter Book](https://firebook.ltpy.adamplatform.eu/) online. For those who want to execute the workflows, the training course can also be accessed in an interactive [JupyterLab platform](https://fire.adamplatform.eu), where the required Python libraries and data are pre-installed. data users can also set-up the same environment on their local machines by cloning the [GitLab repository](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring) and using the environment.yml file provided to install the required libraries.  

# Course Content
The course comprises of two main case studies, each with multiple parts that focus on different phases of the fire life cycle: 

### Wildfires in California, USA 2020
This two-part case study introduces upcoming data products from the MTG and Metop-SG satellite missions in the context of the 2020 August Complex fires which occurred in California, USA. The workflow notebooks are in the folders [ca_part1_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/ca_part1_workflows) and [ca_part2_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/ca_part2_workflows).

Part One of the case study in [ca_part1_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/ca_part1_workflows) focuses on fire monitoring applications using data products from the MTG mission. Part Two of the case study in [ca_part2_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/ca_part2_workflows) introduces users to new capabilities in monitoring smoke transport using data products from the Metop-SG mission.

### Mediterranean fires in Greece and Italy, 2021
This three-part case study introduces upcoming data products from the MTG and Metop-SG missions in the context of the summer wildfires which occurred in southern Italy and Greece in early August 2021. The workflow notebooks are in the folders [med_part1_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/med_part1_workflows), [med_part2_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/med_part2_workflows) and [med_part3_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/med_part3_workflows). 

Part One of the case study in [med_part1_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/med_part1_workflows) introduces data users to forecasting the pre-fire risk using data products whose capabilities will be improved through data from MTG and Metop-SG. With a similar goal, Part Two of the case study in [med_part2_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/med_part2_workflows) focuses on monitoring the active fire phase of the fire life cycle. Finally, Part Three of the case study in [med_part3_workflows](https://gitlab.eumetsat.int/eumetlab/atmosphere/fire-monitoring/-/tree/master/med_part3_workflows) focuses on assessing post-fire impacts.

# Teaching Experience

The FANGS training course was completed in spring 2022. Since then, the notebooks have been used in more than six [EUMETSAT training activities](https://training.eumetsat.int/), reaching over 450 people in 2022. Examples of training activities include workshops at conferences and online webinars with an instructor introducing the case studies and workflows. The training course also allows for self-paced learning as data users can choose what parts of the fire life cycle they wish to focus on and how in-depth they want to go in terms of understanding the workflows. 

# Acknowledgements

FANGS has been supported by the Copernicus Programme through EUMETSAT. We acknowledge contributions from Carla Barrosso (EUMETSAT) and Stephan Bojinski (EUMETSAT).

# References
