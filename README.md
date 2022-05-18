# ESC403 group project 
https://github.com/maverbiest/esc403_olfaction


# The nose knows: comparing olfaction at different concentrations
### Group members: Wei-Chen Kao, Alex Plüss, Nadja Greter, Max Verbiest

Code repository for Olfaction group project in the Introduction to Data Science UZH course ESC403 (2022)

### Data
The data that was used for this project was taken from the 'DREAM olfaction challenge'. The wiki page of this challenge contains extensive information on the aims of the challenge and the types of data that were used. Below is a brief summary of the contents of the data table that was used for our group project.

**data/TrainSet.txt:** Size: 27 variables, 35084 observations ( (338 odors + 20 repeated odors) x 2 concentrations x 49 individuals )

Brief description of columns:
- Compound Identifier: PubChem Compound Identification
- Odor: Synonym for the chemical. May not be unique: for identifying the odor, the CID and not the odor name should be used.
- replicate: Whether the stimulus is part of the 20 stimuli that were tested twice.
- intensity: Whether the data is for the odor at high intensity or at low intensity.
- dilution: Dilution of the odor. Each odor is presented at two different dilutions. 
- subject #: Subject identifier, a number from 1 to 49.
- Intensity/Strength: Perceptual data about how intense or strong the smell was perceived by the subjects. Subjects used a scale from 0-100 where 100 is “extremely strong” and 0 is “extremely weak”.
- Valence/Pleasantness: Perceptual data about how pleasant or unpleasant the smell was perceived by the subjects. Subjects used a scale from 0-100 where 100 is “extremely pleasant” and 0 is “extremely unpleasant”.
- Columns 9-27 contain data in which subjects matched their perception of how the odor smelled to a standard list of 19 perceptual descriptors: bakery, sweet, fruit, fish, garlic, spices, cold, sour, burnt, acid, warm, musky, sweaty, ammonia/ruinous, decayed, wood, grass, flower, chemical. Subjects used a scale from 0-100 where 100 is “very much” and 0 is “not at all”.

### Notebooks generated for analysis
These can be found in the 'notebooks' folder in this repo.

**notebooks/part0_eda.ipynb:** Some exploratory analysis on the TrainSet.txt data

**notebooks/part1_perceived_strength_umap_mv.ipynb:** Investigating how the intensity of perception changes between high and low concentration data.

**notebooks/part2_Correlation_descriptors_pleasantness_nrg.ipynb:** Which descriptors are correlated to perceived pleasantness? Is this the same at high and low concentrations?

**notebooks/part3_pleasantness_across_subjects_wck.ipynb:** Do all subjects enjoy the same odors? Is this the same at high and low concentrations?

**notebooks/part4_olfaction_ajp.ipynb:** Can we train a model to predict the perceived pleasantness of an odorant based on it's descriptions? Is this the same at high and low concentrations?


