# Machine Learning to Make KPI of a Power Plant


Title: Developing robust key performance indicators (KPI's) for the base utility power plant by employing machine learning on readily available data.

Key performance indicators (KPI) dashboards for the chemical and energy assets at the disposal of operators and manager can help in monitoring and improve efficiency. Reliable and robust deployment of the KPI's in the form of dashboards with predictive features can help plan in the decision making of future operations. Thermodynamic and first principle based models for chemical and energy plants consist of a complex system of non-linear equations. The solution of such models requires computing resources and time, which make them unsuitable for the robust deployment of KPI dashboards. Machine learning (ML) can be an alternative approach for developing models for such assets. It would ease deployment if the ML models use readily available sensor data and historic operation data. 

In this project ML approach is demonstrated to predict net power output of base utility combined cycle power plant (CCPP). The CCPP consist of a gas turbine (GT), steam turbine (ST), and heat recovery steam generators (HRSG). This type of power plant is being installed in increasing numbers around the world where there is access to substantial quantities of natural gas [1].

Gas turbine power output primarily depends on the ambient parameters which are ambient temperature, atmospheric pressure, and relative humidity. Steam turbine power output has a direct relationship with vacuum at exhaust [2]. Building on that four parameters that are readily available in a CCPP are selected: ambient temperature (AT), ambient pressure (AP), relative humidity (RH), and exhaust vacuum (V).

Operating data of power plants is the proprietary of the asset owners and/or design companies and public access is limited. For this project data was obtained from UCI repository for a CCPP located in turkey [3]. The data was collected over the time of 6 years.  

The development of KPI was demonstrated using data analysis and regression tools. In the data analysis, data was loaded as pandas data frame and its features were explored. The correlation among the parameters was plotted as grid plot to find out independent nature of the data, results are shown in the jupyter notebook Q3_Plot1.ipnyb. For regression, the data was split into two sets: train set and test set. A linear regression model was trained on the train set and results were evaluated by comparing with the test set. The predicted PE values were plotted against the measured ones and goodness of prediction measures such as MAE, MSE, and RMSE were calculated.  Jupyter notebook Q3_Plot2 shows the results.

Overall the two plots of this exercise show that the EP (a KPI measure) of a CCPP can be predicted using external readily available data with reasonable accuracy. This approach can be extended to more KPI measures and for other chemical and power plants. For this purpose, more test data and ML algorithm need to be evaluated. 

References:
	1. Ramireddy V. An overview of combined cycle power plant. <http://electricalengineering-
portal.com/an-overview-of-combined-cycle-power-plant> [accessed: 02.03.13].
	2. Tüfekci P. Prediction of full load electrical power output of a base load operated combined cycle power plant using machine learning methods, Electrical Power and Energy Systems, 60, 126–140, 2014.
	3. http://archive.ics.uci.edu/ml/datasets/Combined+Cycle+Power+Plant [accessed 03.02.2018]
