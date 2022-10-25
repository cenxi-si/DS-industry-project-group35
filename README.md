# DS Industry Project Group35

# Testing the Causality between Online and Offline Behaviours

## Collective Team Details (Member's Name/Student ID)
- Cenxi Si 1052447
- Manish Kumar Shaw 1230045
- Guoan Wang 1146487
- Keang Xu 1008807


## Description
According to research carried by Branley and Covey, it concluded that the exposure of risky information online would lead to users engaging risky offline behaviors. Also, the World Health Organization said that the violence against women, especially domestic violence is still shockingly widespread. In this study, we mainly focus on the misogynist related information posted online which represents the online behavior. Due to the survey data cannot be used to test causation, the time series data is worth to generate. Thus, in this project, we mainly focus on using convergent cross mapping to study the causality between domestic crime and misogynist tweets from 2012 to 2020 in the US.

Our project is hosted by the University of Melbourne, and our client is Prof. Simon Dennis. To make a hypothesis, there would be a direct causality between domestic crime and misogynist tweets. However, if the causality is insignificant at the end, other factors including alcohol establishments, cost of living and temperature changes will be analyzed towards crime and tweets to see whether they could affect them indirectly.

To make sure everyone is familiar with the procedure of building CCM model, each of us took the responsibility of one variable and analyze the causality with crime and tweets respectively.


## Files
- data: all related data are in the data folder
- data_preprocessing: it includes the codes for preliminary data cleaning and preprocessing
- CCM_Alcohol.ipynb: it is the notebook for alcohol establishment variable under CCM
- CCM_cost_of_living.ipynb: it is the notebook for cost of living variable under CCM
- CCM_MisogynyTweet_vs_RapeCount.ipynb: it is the notebook for misogynist tweets variable under CCM
- CCM_Temperature.ipynb: it is the notebook for temperature variable under CCM
- Meeting_minutes: all meeting minutes in semester 1 and 2 are included here
- drafts: this folder is for all the useless information
