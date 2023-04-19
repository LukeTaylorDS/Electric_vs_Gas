# Seattle Collision Data


##
## Data Overview
For our Project, we pulled the data from Data.gov for Vehicle Collisions from 2003 to present for the City of Seattle. 
##

## Tableau Information
https://public.tableau.com/app/profile/tayler.despain/viz/CityofSeattleReportedVehicleAccidents/Dashboard1
https://public.tableau.com/app/profile/ivan.david.quesada/viz/seattleaccidentsplt/DUIdash?publish=yes
https://public.tableau.com/app/profile/ivan.david.quesada/viz/seattleaccidentsplt/speeddash?publish=yes
https://public.tableau.com/app/profile/ivan.david.quesada/viz/seattleaccidentsplt/minmaxdash?publish=yes
https://public.tableau.com/app/profile/ivan.david.quesada/viz/seattleaccidentsplt/weatherandcollisiontypedash?publish=yes
##

### Predicting Falities and Serious Injury using Machine Learning

#### What is the purpose of being able to predict whether a collision will cause serious injuries or fatalities?
Being able to accurately predict collision fatalities can have several potential benefits:

* Prevention and mitigation of accidents: If a model can accurately predict whether a collision is likely to result in fatalities, it can help in taking preventive measures to avoid such accidents or mitigate their severity. For example, if a collision is predicted to be highly likely to result in fatalities, emergency response teams can be dispatched quickly to the accident site, potentially saving lives through prompt medical attention.
* Resource allocation and planning: Predicting collision fatalities can help with resource allocation and planning for emergency services and medical facilities. For instance, hospitals and trauma centers can prepare for a potential influx of critically injured patients, ensuring that adequate resources and personnel are available to handle the situation effectively.
* Traffic safety and infrastructure planning: Insights gained from predicting collision fatalities can inform traffic safety policies and infrastructure planning. For example, identifying high-risk locations or road conditions associated with a higher likelihood of fatalities can lead to targeted interventions, such as improving road signage, adding traffic control measures, or implementing road safety campaigns in those areas.

Overall, accurately predicting collision fatalities can have significant societal benefits by potentially saving lives, improving traffic safety policies and infrastructure, and informing emergency response and resource allocation strategies.

#### Ok, so what did you build and does it work?
After spending several hours cleaning and preprocessing a messy and unusable CSV file with over 50 columns and nearly 250,000 rows, I successfully extracted relevant features such as light conditions, weather conditions, road conditions, and collision severity. I then performed exploratory data analysis (EDA) to gain insights into the data and built and trained a machine learning model to predict collision fatalities based on these features. 

The machine learning model was trained using a supervised learning approach, where historical collision data was used to train the model to predict the likelihood of a collision resulting in fatalities and serious injuries. The model was evaluated using various performance metrics such as accuracy, precision, recall, and F1 score to assess its effectiveness in predicting collision fatalities.

#### What machine learning algorithm did you choose and why?
We chose to go with the Random Forest Classifier algorithm because not only did it show high performance, it also;
* Provides a feature importance measure, which allows for the identification of the most important features in the dataset. This can help in understanding the underlying patterns and relationships in the data, and make informed decisions based on feature importance rankings. 
* Can capture non-linear relationships and interactions between features in the data, making it suitable for complex datasets where simple linear models may not perform well.
* Can handle large datasets and high-dimensional feature spaces efficiently, making it suitable for datasets with a large number of samples or features.
![Alt text](images/ml_performance_metrics.png)

Based on the evaluation results, the model showed promising performance with high accuracy and reasonable precision, recall, and F1 score. When evalutating other models we looked for the high recall scores, meaning we wanted something that caught as many true negatives as possible.
![Alt text](images/ml_bfc_confusion_matrix.png)

## Presntation Slides
https://docs.google.com/presentation/d/1NGh0JGHu3NgqyXn_sbl0Y530mmzCxedCYg6hrpIQaPc/edit#slide=id.g219bedc804f_0_20
