# The Irish Social Vulnerabiltiy to Environmental Hazards Index (ISVEHI)
The ISVEHI is a spatial assessment of the social vulnerability of Ireland’s population to climate-related hazards (e.g. flooding, (coastal, fluvial, and pluvial), coastal erosion, strong wind/storms, heatwaves). Social vulnerability is “the sensitivity of a population to natural hazards and its ability to respond to and recover from the impacts of hazards”.
The index has been developed using a total of 22 indicators representing attributes, such as age, health, education level, local knowledge. These indicators were combined with equal weighting and mapped at the CSO small area scale with each small area being assigned a social vulnerability score. An example of the spatial output for Dublin can be seen below.

<p align="center">
<img src="images/dublin.jpg" width="600">
</p>

This repository supports the journal publication Fitton, J.M., O'Dwyer B., Maher, B. (2021) 'Developing a social vulnerability to environmental hazards index to inform climate action in Ireland/ Irish Geography' Vol. 54, No. 2 November 2021, DOI:10.2014/igj.v54i2.1468.

# Why has the ISVEHI been created?
Ireland’s climate is changing. Observations show evidence of higher temperatures, rising sea levels, and changing patterns of precipitation, with trends expected to continue and intensify into the future. Consequently, an increase in the occurrence and intensity of fluvial and coastal flooding, coastal erosion, drought, and heatwaves are expected. 
These hazards can impact upon people and assets, and depending on the severity, may cause a loss of life or damage to key infrastructure. Risk assessments are therefore needed to understand the risks posed by these hazards to inform adaptation. 

The Intergovernmental Panel on Climate Change (IPCC), define risk as comprising three components: a hazard, exposure to the hazard, and vulnerability. In Ireland, data and information on future climate change, hazards, and assets that are potentially exposed are available already. However, to date, there has been no national assessment of vulnerability to environmental hazards within Ireland.   

To begin to address the social vulnerability knowledge gap in Ireland, the Irish Social Vulnerability to Environmental Hazards Index (ISVEHI) has been developed.

# The Code
The ISVEHI was created using ‘R’ and data from the CSO Census and Copernicus. The easiest way to run the code is via a conda environment.

The environment mimics the R environment that the code was developed upon, therefore allowing the code to run without errors. This environment is created and managed using [Anaconda](https://www.anaconda.com). The following instructions will guide you through the steps to install Anaconda and use the code.

**Step 1: Download ISEVHI:** Clone or download the ISEVHI repository from GitHub using the button 'Clone or Download' above and save it somewhere locally on your computer, e.g. C:\ISEVHI.

**Step 2. Anaconda:** Install [Anaconda](https://www.anaconda.com/download/). Open the Anaconda prompt (PC) or on a Mac or Linux system open a terminal window. Use the `cd` command to change the directory, and navigte to go the folder where you have downloaded the ISEVHI repository (see [here](https://www.digitalcitizen.life/command-prompt-how-use-basic-commands) for information on how to use the command prompt).

**Step 3: Create a new environment:** Create a new environment named `ISEVHI` with all the required packages:

```
conda env create -f environment.yml -n ISEVHI
```

This environment should ensure that all the required packages are installed. This environment is called `ISEVHI`. The next step is to active the environment in the command prompt with:

```
conda activate ISEVHI
```

The terminal command line prompt should now have changed from (base) to (ISEVHI).

## How to use the scripts

The code is written in [Jupyter Notebooks](https://jupyter.org/). This is a "web-based interactive development environment" and allows for comments and descriptions to be added to the code to support/aid understanding.

Ensure that you have navigated to the ISEVHI directory within the  anaconda prompt, e.g. C:\ISEVHI, then type:

```
jupyter notebook
```

This will then open a web browser, and you should be able to see the files within the C:\ISEVHI directory. The files then end with .ipynb contain the scripts. For more information on how to use Jupyter Notebooks, see this [video](https://www.youtube.com/watch?v=HW29067qVWk).

You should use the scripts in the following order:
1. 0_Scripts/1a_CensusData.ipynb
2. 0_Scripts/1b_PopulationDensity.ipynb
3. 0_Scripts/1c_imperviousSurfaces.ipynb
3. 0_Scripts/1d_combineVulnerability.ipynb

# Support

If you are having a problem, please create a new [Issue](https://github.com/jamesfitton/ISVEHI/issues). This keeps all problems and solutions in the same place and acts as a resource for other users to address the same/similar problems.



 
 
