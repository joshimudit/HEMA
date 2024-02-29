# Literature Review

**Central idea**: 

**Summary of Each Work**:

- **Source 1**: Skeels et al. 2021 (Background concept)

  - **[Link](https://doi.org/10.1093/sysbio/syac048)**
  - **Concept 1**: The evolution of Earth’s climate on geological timescales is largely driven by variations in the magnitude of total solar irradiance (TSI) and changes in the greenhouse gas content of the atmosphere.
  - **Concept 2**: Evolutionary Speed Hypothesis ESH predicts that environmental kinetic energy shapes variation in speciation rates through temperature or life history-dependent rates of evolution.
  - **Relation to the Project**: This paper establishes the background that the evolution of biodiversity on earth is dependent on Global average temperature and pCO2 conc. (greenhouse gas).


- **Source 2**: Foster et al. 2017 (Source of climate data)

  - **[Link](https://doi.org/10.1038/ncomms14845)**
  - **Objective**: To track the evolution of climate on earth based on different other scientific research. This shows the maximum probability scenario of climate that occurred.
  - **Methods**: The CO2 curve derived from this literature becomes the source of other 2 hypothetical climate scenarios, the median CO2 one and extreme CO2 in the mass extinction scenario.
  - **Relation to the Project**: This is basis of 3 climatic scenarios, _maxprob_ (for model training), _median_ and _mext_ (for making predictions)


- **Source 3**: Hagen et. al. 2021 (Input data source - of species richness, for model training)

  - **[Link](https://doi.org/10.1371/journal.pbio.3001340)**
  - **Objective**: R-based simulation model engine, to track the eco-evolution of species over various spatial and temporal scales.
  - **Methods**:  mechanistic modeling
  - **Outcomes**: I used this R model to generate simulated Species Richness data for the maximum probability climate scenario.
  - **Relation to the Project**: We use this Species richness data to train the model (as target), and then this model is used to predict species richness in other 2 climatic scenarios.
 


- **Rationale & Research question**

  - the R-based _gen3sis_ model is a complex mechanistic model in nature, it is computationally very expensive for the evolution of Species richness (SR) based on climate reconstructions. The idea is to find if neural networks can be used to predict SR in a relatively quicker way.
  - In this project, the idea is to train a Neural network on a simulation dataset and use it to predict species richness in different
hypothetical climate scenarios:
    - Maximum probability pCO2 ( Froster et. al 2017 ) Used for model training
    - Median pCO2 constantly over time
    - Mass extinction scenarios, with extreme peaks of pCO2




- **Objectives**
      - Data import and preparation
      - Visualization of Data, Selection of Features and Target Variable
      - Making a Baseline model (Regression Neural Network)
      - Tuning Hyperparameters to build Robust model architecture.
      - Using this model to predict Species Richness in new scenarios.
