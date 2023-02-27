# Investigating a Gulf Stream Frontal Eddy North of Cape Hatteras: Questioning Overall Impacts on Ecology

Authors:
[Patrick C. Gray](https://orcid.org/0000-0002-8997-5255) Jessica Gronniger, Ivan Sayvelev, Julian Dale, Alexandria K. Niebergall, Nicolas Cassar, Anna E. Windle, Dana E. Hunt, Zackary Johnson, Marina Lévy, Chris Taylor, Guillaume Bourdin, Ashley Blawas, Amanda Lohmann, Greg Silsbe, David W. Johnston

This is currently available on bioRxiv at: https://doi.org/10.1101/2023.02.22.529409 and is under review at the Journal of Geophysical Research: Oceans.

### Running the Notebooks
Once you have pulled the repo down locally via git and have Docker installed all code here can be run fully in Docker based on a prebuilt environment by running:

`docker run -it -v <location of code>:/home/jovyan --rm -p 8888:8888 pangeo/pangeo-notebook:2021.05.15 jupyter lab --ip 0.0.0.0`

This will launch a Jupyter Lab instance that can run everything for you. This can also be easily done in the cloud if you have a cloud environment that can be launched with a Docker image.

All the data for this work is included on Zenodo at doi.org/10.5281/zenodo.7680135 and should be placed within this repo in a directory called `data/` but this can be changed with a variable at the beginning of each notebook.

## Plain Language Summary of this Work

Frontal eddies are spinning masses of water (~30km in diameter) that move along western boundary currents like the Gulf Stream. When they form they carry productive coastal water into the Gulf Stream and drive upwelling within their cores. Together this leads to an increase in the amount of phytoplankton within them - much higher compared to surrounding nutrient-limited Gulf Stream water. On the east coast of the United States one common area of frontal eddy formation is just off Charleston, SC. Eddies then travel up the coast and dissipate near Cape Hatteras, NC. In this work we measured a wide range of physical and biological properties of a frontal eddy just north of Cape Hatteras. We compared these properties within the eddy to the coastal water on one side and the Gulf Stream water on the other, finding clear differences in phytoplankton community composition and other physical and chemical properties. Using the results of these observations together with previous studies we share a simple model for how frontal eddies may impact phytoplankton, zooplankton, and fish – hypothesizing that they may contribute to the high diversity and density of top predators off Cape Hatteras.

### The key points of this work are:
- In-depth investigation of a frontal eddy in the Gulf Stream off Cape Hatteras, North Carolina
- Continued physical and biogeochemical differences are observed between the eddy and adjacent water masses even as it begins to shear apart
- A conceptual model is developed for the ecological impact of frontal eddies along with the hypothesis that they could supply zooplankton to secondary consumers

### Notebooks
There are a number of notebooks that can be used to recreate this analysis along with the provided data: 
- In analyze_sw_cruise_all_inline.ipynb we do most of the primary analysis which analyzes all and combines nearly all the primary datasets and then compares them discretely and on T-S diagrams. It also visualizes the ACS data and many of the supplemental figures.
- In analyzing_adcp_data.ipynb we generate the ADCP echosounder comparisons and visualizes four transects across the frontal eddy with all the ADCP data. 
- In profile_analysis_sept.ipynb we calculate the mixed layer depths and visualizes the profile data.
- In acs_analysis_sept_cruise.ipynb we visualize the ACS data across all transects and ensure data quality.
- In olci_sat_analysis.ipynb we generate all the satellite data comparison and look at the frontal eddy over time.
- In analyze_sw_cruise.ipynb we just explore both the satellite data and the ship data.
- In processing_sept_ctd.ipynb we show all CTD data from the cruise.
- In model_output_analysis.ipynb, which is not included in the paper, we compare satellite data to model output to see if the eddy is represented in a high resolution model.
- In format_for_inline_analysis.ipynb we take the Seabird and ship system output and merge it into a usable .csv file.


### Citation
https://doi.org/10.1101/2023.02.22.529409
