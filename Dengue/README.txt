=================================================================
=			Predicting Dengue Cases Using Climate Data			=


= Data Exploration and comparison of different modeling approaches
= on varioius climate features collected by multiple US Departments.
= Datasets provided for the cities of Iquitos, Peru and San Juan, Puerto Rico

= Based off of the dengue forecasting competition held by these departments
= https://dengueforecasting.noaa.gov

= -- Currently a DrivenData.org competition
= https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread

== Folder Structure:
= data: CSV of raw data and any pickled dataframes from notebooks

= Data storytelling: EDA notebook and txt file of dictionary explaining ind. variables

= Dengue statistics: Notebook for hypothesis testing, precipitation and average air tempurature

= models: modeling notebooks with explanatory graphics, ARIMA, Linear Regression, GradientBoosting family models, and intermediate scrap notebook with different approaches tried

= reports: documentation and write-ups

 
Notebooks are run in sequence:
	Dengue_Data_story.ipynb (read CSVs, feature and target exploration, some processing) -> pickle dataframes
	> LinearModels.ipynb (month dummy variables, feature transformation, imputation) -> pickle transformed dataframes
	
	Suggested sequence afterwards: ARIMA_Models.ipynb > GradientBoosting.ipynb
		*After first 2 notebooks, the rest of the modeling notebooks can be run in any order
		
	Dengue_statistics.ipynb can be run after Dengue_Data_story.ipynb is run for pickles
	
		
