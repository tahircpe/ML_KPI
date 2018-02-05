Title: Developing robust key performance indicators (KPI's) for the base utility power plant by employing machine learning on readily available data.

Key performance indicators (KPI) dashboards for the chemical and energy assets at the disposal of operators and manager can help in monitoring and improving efficiency. Reliable and robust deployment of the KPI's in the form of dashboards with predictive features can help plan in decision making of future operations. Thermodynamic and first principle based models for chemical and energy plants consist of a complex system of non-linear equations. Solution of such models requires computing resources and time, which make them unsuitable for the robust deployment in KPI dashboards. Machine learning (ML) can be an alternative approach for developing models for such assets. It would ease deployment if the ML models use readily available sensor data and historic operation data. 

In this project ML approach is demonstrated to predict net power output of base utility combined cycle power plant (CCPP). The CCPP consist of gas turbine (GT), stream turbine (ST), and heat recovery steam generators (HRSG). This type of power plant is being installed in increasing numbers around the world where there is access to substantial quantities of natural gas [1].

Gas turbine power output primarily depends on the ambient parameters which are ambient temperature, atmospheric pressure, and relative humidity. Steam turbine power output has a direct
relationship with vacuum at exhaust [tfecki]. Building on that four parameters that are readily available in a CCPP are selected: ambient temperature (AT), ambient pressure (AP), relative humidity (RH), and exhaust vacuum (V).

Operating data of power plants is the proprietary of the asset owners and/or design companies and public access is limited. For this project data was obtained from UCI repository for a CCPP in located in turkey [UCI link]. The data was collected over the time of 6 years. 

1. Ramireddy V. An overview of combined cycle power plant. <http://electricalengineering-portal.com/an-overview-of-combined-cycle-power-plant> [accessed: 02.03.13].

2. Tüfekci P. Prediction of full load electrical power output of a base load operated combined cycle power plant using machine learning methods, Electrical Power and Energy Systems, 60, 126–140, 2014.
