🚀 WATER QUALITY ANALYSIS USING MACHINE LEARNING


📌Introduction

Water quality analysis plays a crucial role in assessing the suitability of water for various purposes, including drinking, agriculture, and industrial use. This project focuses on analyzing key water quality parameters such as Residual Sodium Carbonate (RSC), pH level, and Total Dissolved Solids (TDS) using machine learning techniques. The analysis aims to understand the distribution of these parameters, their significance in assessing groundwater quality, and potential correlations between them.

📌Dataset Description

The dataset used for this analysis includes water quality measurements collected from various regions over multiple years. It contains information on parameters such as RSC, pH, TDS, geographical location, and classification of water quality. Preprocessing steps involve handling missing values and encoding categorical variables.

📌Analysis of RSC

Summary:
The dataset's mean RSC value is approximately -2.36, and the median is around -1.36, both significantly below the acceptable range of 1.25. The most common RSC value is -0.60. District-wise analysis reveals poor RSC values in Kumuram Bheem and Mulugu districts, emphasizing the need for local authorities to address groundwater quality. RSC values vary yearly, with 2020 showing the highest variation, particularly during post-monsoon seasons, where values often exceed acceptable limits, demanding targeted management strategies.
Visualizations:
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/f8406918-5c8a-453e-916e-b4e34f1355af)

![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/6b4b2b95-2c96-4424-a562-edf9a2946b4b)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/b73d8419-b5c1-4b81-a8bf-308ee41341b8)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/2143c19c-8b42-4655-8403-fdc200af0c5c)




📌Analysis of pH

Summary:
pH in groundwater reveals that the water is generally slightly alkaline with a central tendency around pH 8. There is a slight shift in the pH in Nagarkurnool i.e 7 .  Notably, pH varies among water quality classes and districts, implying localized differences in water quality that warrant attention. However, pH remains stable over time, indicating consistent underlying factors. Seasonal analysis suggests that the water maintains its alkaline nature throughout the year.
Visualizations:
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/8937428a-3d09-4fcd-ac0b-ec981af4913e)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/2225d8de-5d11-4076-b546-479df70a1197)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/913c29bf-1f04-4186-8b7f-c774613a2c9a)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/8c091d6d-87cb-42f1-aabc-ccc5a062c2b1)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/ee7767a7-25c8-4cad-8d8a-dcfb2f51a276)






📌Analysis of TDS
Summary:
 Most TDS values fall within the 'Excellent' to 'Very Satisfactory' range, affirming the suitability of water for consumption, meeting safe drinking water standards.DS values remain consistently 'Excellent' over the years, ensuring a dependable source of drinking water.  The majority of districts boast 'Excellent' to 'Very Satisfactory' TDS values, underscoring the widespread availability of high-quality water resources. TDS values consistently stay within acceptable ranges across seasons, reducing the necessity for seasonal variations in water treatment.Specific water quality classes, such as C4S2, C4S1, C4S4, C4S3, and C3S3, consistently exhibit 'Very Satisfactory' TDS values. This information can guide precise policy interventions to address water quality concerns in regions with lower TDS levels.

Visualizations:
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/23baadbe-75a2-4db8-9ee9-783c106aee10)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/6e5bde89-5a36-4285-9ca2-b02f0c9306e7)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/d38b015d-77e3-49c1-9a31-decedabe33dc)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/9b5cdee5-6b70-4e2a-9dce-622b187fe27f)
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/7f30d378-1c96-42d9-90bf-78e59bb55f43)






📌Correlation Analysis
Correlations:
Explore correlations between RSC, pH, and TDS values to identify relationships and potential dependencies between water quality parameters.
Correlation Heatmap: Visualize correlations between variables to understand the strength and direction of relationships.
![image](https://github.com/Prakriti2901/Water-Quality/assets/122342001/114ee1dc-b28b-45ec-abe3-1429feaa3aef)



📌Machine Learning Approach (if applicable)
Algorithms Considered: Logistic Regression, K-Nearest Neighbors (KNN), Artificial Neural Network (ANN)
ANN-
We have divided the dataset as 80% for training and 20% for testing. 
In our model we have 5 layers.
The first layer being the input layer, we channel 18 features and 80% of data rows for training the model. 
It propagates to the next hidden layer after getting processed by the relu function. The next layers receive half the previous input till the fourth layer. At the last layer the input is reduced to nine, as we have nine classes for water quality. The final layer gives predictions for the water quality with an accuracy around 90%.

The accuracy could be further improved by increasing the complexity of the model by adding more layers or using other activation functions. Moreover, accuracy could be better if more data were available to train the model.

LOGISTIC REGRESSION-
We implemented the logistic regression model imported from SciKitLearn packages. We used parameters of year, gwl, pH, E.C, TDS, CO3, HCO3, Cl, F, NO3, SO4, Na, K, Ca, Mg, T.H, SAR, RSC to predict classification. The model score is 0.93 on the testing data (0.2 of the dataset). We have considered the random state while splitting the dataset as 42.  

📌Conclusion
The analysis of water quality parameters using machine learning techniques provides valuable insights into the state of groundwater quality and its implications for various stakeholders. By understanding the distribution, trends, and correlations between key parameters, informed decisions can be made to improve water resource management practices and safeguard public health.

📌Future Work
The dataset provides a valuable foundation for future research and policy development. 
Long-Term Trends: Analyzing data over several years can reveal long-term trends in groundwater quality, helping policymakers anticipate future challenges.
Impact Assessment: Research can be conducted to assess the direct impact of groundwater quality on crop yields, livestock health, and human well-being. 
Water Management Strategies: Developing strategies for sustainable water management, including water treatment and irrigation practices, can help optimize the use of available groundwater resources.
Awareness Campaigns: Future initiatives can include awareness campaigns for farmers and local communities to promote responsible water usage and conservation.



📌Acknowledgements
Data Sources: https://www.kaggle.com/datasets/sivapriyagarladinne/telangana-post-monsoon-ground-water-quality-data/code?select=ground_water_quality_2018_post.csv
Libraries Used: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow, Keras


References
[[Include citations for research papers, articles, or resources referenced in the analysis.]](https://www.sciencedirect.com/science/article/pii/S1532046403000340

https://bmcmedinformdecismak.biomedcentral.com/articles/10.1186/1472-6947-5-3

https://www.mdpi.com/2076-3417/10/17/5776

https://iwaponline.com/wqrj/article/53/1/3/38171/Water-quality-prediction-using-machine-learning

https://www.mdpi.com/2073-4441/11/11/2210
)

