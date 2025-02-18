### Remote Sensing Modeling

**David House**

#### Executive summary


#### Rationale
These methods could allow for eventual deforestation tracking, oil spill monitoring in the ocean or other tasks that require finding changes in the environment.

#### Research Question
Can unsupervised machine learning methods make a map of ground cover types to identify areas of interest?

#### Data Sources
[LandSat 8 Data](https://earthexplorer.usgs.gov/)

#### Methodology
Initial investigations consist of using the Bands of LandSat images as features for unsupervised machine learning models. This could allow for automated systems to monitor changes in the ground cover of a certain region.

#### Results
Initial findings show there are correlations between the bands and there seems to be different slopes based on the pixel in question. 

The K Means method seemed to separate water, dry region and forests.

The HDBSCAN method separated ocean, lakes, dry regions and forests.

The fact that oceans and fresh water was difficult for K means clustering implies that they are close in the feature space, but there is enough of a difference for HDBSCAN to pick it up.

#### Next steps
At the end of the notebook I have added domain knowledge conversions that could prove useful in honing the model for specific ground cover types, such as recently burned or dry areas.

#### Outline of project

- [Notebook](main.ipynb)
- [Findings](Findings.docx)

