
Capstone Project - Refine research question and methodology - Module 16
========================================================================
Refine your problem statement to include a research question, expected data sources and structure, expected results and techniques.


Research Question (Primary)
---------------------------
Which counties in the Permian Basin in the state of Texas are best suited for investment in renewable energy projects and why? What type of projects are suitable to develop in those counties? 

Secondary Research Question:
----------------------------
Using the socio-economic data of the Permian Basin identify top factors that contribute to the lack of internet access for workers in a given county. How will this impact the decision to invest in renewable energy projects in that county?


Background
----------
Renewable energy projects, like wind and solar, offer plenty of investment opportunities in the emerging market for net-zero carbon world. The transition to clean energy is essential to meet the Paris Climate Agreement's goal of reduced carbon emissions by 2030. Eventual goal is to get to net-zero carbon by 2050. This requires major shifts in energy use patterns from hydrocarbon-based resources (oil, natural gas, coal) to renewable energy sources, primarily land-based wind, off-shore wind and solar energy sources. There are also battery energy sources (BESS) as well as distributed wind and solar rooftop commercial and residential opportunities.

This project will explore investment opportunities for renewable energy projects in the Permian Basin area in Texas, USA.

Internet access is critical for long-term viability of deploying renewable energy projects in an area. Internet access allows the local population to learn and develop knowledge and skills for jobs in the renewable industry and also to keep updating skills as the industry develops. To attract new and younger workers to the area, good internet access is normally deemed necessary for investment in renewable energy projects. Lack of internet access can be a negative factor for investment since it impedes worker learning and development.


Data Sources
-------------
The National Renewable Energy Lab (NREL) (https://www.nrel.gov/) is one of the premiere U.S. government research labs that shares information on the use and deployment of renewable energy technologies and projects in the U.S. The NREL Permian Energy Development Lab (PEDL) published a data set for socioeconomic (including energy production) data for all the counties in the Permian Basin in Texas and New Mexico.

The dataset are organized into four categories: Socioeconomics, Health & Wellbeing, Jobs & Workforce, and Energy Infrastructure & Potential. 

Each category contains multiple data elements the details of those are provided in a separate file: nrel_ses_permian_basin_counties_metadata.txt

The metadata related to renewable energy information are provided below for reference - 

	UtilityPV_TechPotential	Technical potential for utility-scale solar by county. Note: Technical potential is a theoretical upper bound for generation potential that considers resource and land availability. It does not consider economic or market feasibility, nor does it consider existing systems.	NREL	2020	
	ResidentialPV_TechPotential	Technical potential for rooftop solar on residential buildings by county. Note: Technical potential is a theoretical upper bound for generation potential that considers resource and rooftop availability. It does not consider economic or market feasibility, nor does it consider existing systems.	NREL	2020	
	CommercialPV_TechPotential	Technical potential for rooftop solar on commercial buildings by county. Note: Technical potential is a theoretical upper bound for generation potential that considers resource and rooftop availability. It does not consider economic or market feasibility, nor does it consider existing systems.	NREL	2020	
	LandbasedWind_TechPotential	Technical potential for utility-scale, onshore wind by county. Note: Technical potential is a theoretical upper bound for generation potential that considers resource and land availability. It does not consider economic or market feasibility, nor does it consider existing systems.	NREL	2020	
	DistributedWind_TechPotential	Technical potential for residential and commercial behind-the-meter wind by county. Note: Technical potential is a theoretical upper bound for generation potential that considers resource and land availability. It does not consider economic or market feasibility, nor does it consider existing systems.	NREL	2020	
	GeothermalHeatPump_EconPotential	Economic potential for geothermal heat pumps (GHPs), also known as ground-source heat pumps, which can provide a renewable source of space conditioning and water heating in buildings. Note: Economic potential is modeled in a conservative, business-as-usual case, which assumes low technology development and conservative customer adoption rates. GHP economic potential represents the sum of the potential GHP applications that result in positive net present value of the investment for each county.	NREL	2020	

Data columns (total 128 columns):
 #    Column                                           Dtype  
---   ------                                           -----  
 0    CountyFIPS                                       int64  
 1    State                                            object 
 2    County                                           object 
 3    PopulationSize                                   int64  
 4    PopulationChangeRate_2010_2020                   float64
 5    PopulationChangeRate_2020_2021                   float64
 6    GDP_2021_thousands                               int64  
 7    GDP_staterank2021                                int64  
 8    GDP_pctchange_2020_2021                          float64
 9    GDP_pctchange_staterank2021                      int64  
 10   TribeName                                        object 
 11   TribeAcres                                       float64
 12   DAC_StatusYES_NumTracts                          int64  
 13   DAC_StatusYES_PctTracts                          float64
 14   SVI_OverallRanking                               float64
 15   SVI_Socioeconomic                                float64
 16   SVI_HouseholdCharacteristics                     float64
 17   SVI_MinorityStatus                               float64
 18   SVI_HousingTransportation                        float64
 19   PctAge65andOlder                                 float64
 20   PctUnderAge18                                    float64
 21   PctBlackNonHispanic                              float64
 22   PctHispanic                                      float64
 23   PctNativeAmerican                                float64
 24   PctWhiteNonHispanic                              float64
 25   PctMultipleRace                                  float64
 26   PctLimitedEnglishSpeaking                        float64
 27   PctForeignBorn                                   float64
 28   PctLessThanHS                                    float64
 29   PctHSDiplomaOnly                                 float64
 30   PctSomeCollege                                   float64
 31   PctAssocDegree                                   float64
 32   PctCollegePlus                                   float64
 33   MedianHHInc                                      float64
 34   PovertyRate                                      float64
 35   EnergyBurden                                     int64  
 36   UnemploymentRate                                 float64
 37   Literacy_AvgScore                                float64
 38   Literacy_PctLevel1                               float64
 39   Literacy_PctLevel2                               float64
 40   Literacy_PctLevel3                               float64
 41   Numeracy_AvgScore                                float64
 42   Numeracy_PctLevel1                               float64
 43   Numeracy_PctLevel2                               float64
 44   Numeracy_PctLevel3                               float64
 45   HealthRank_HealthOutcomes                        object 
 46   HealthRank_LengthOfLife                          object 
 47   HealthRank_QualityOfLife                         object 
 48   HealthRank_HealthFactors                         object 
 49   HealthRank_HealthBehaviors                       object 
 50   HealthRank_ClinicalCare                          object 
 51   HealthRank_SocialEconomicFactors                 object 
 52   HealthRank_PhysicalEnvironment                   object 
 53   Cancer_PctTractsOver75thPctile                   float64
 54   Respiratory_PctTractsOver75thPctile              float64
 55   DieselPM_PctTractsOver75thPctile                 float64
 56   PM25_PctTractsOver75thPctile                     int64  
 57   Ozone_PctTractsOver75thPctile                    float64
 58   LeadPaint_PctTractsOver75thPctile                float64
 59   NPL_PctTractsOver75thPctile                      float64
 60   RMP_PctTractsOver75thPctile                      float64
 61   TSDF_PctTractsOver75thPctile                     float64
 62   UST_PctTractsOver75thPctile                      float64
 63   Wastewater_PctTractsOver75thPctile               float64
 64   ClimateLifeLoss_PctTractsOver75thPctile          float64
 65   Uninsured_PctTractsOver75thPctile                float64
 66   FoodDesert_PctTractsOver75thPctile               float64
 67   NoInternet_PctTractsOver75thPctile               float64
 68   Over30minCommute_PctTractsOver75thPctile         float64
 69   AvgCommute_mins                                  object 
 70   TotalWorkforce                                   int64  
 71   FossilEmpRank_PctTractsOver75thPctile            int64  
 72   CoalEmpRank_PctTractsOver75thPctile              int64  
 73   PctEmpExtraction                                 float64
 74   PctJobs_ManagementBusinessFinancial              float64
 75   PctJobs_ComputerEngineeringScience               float64
 76   PctJobs_EducationLegalArtsMedia                  float64
 77   PctJobs_Healthcare                               float64
 78   PctJobs_Service                                  float64
 79   PctJobs_SalesOffice                              float64
 80   PctJobs_NaturalResourcesConstructionMaintenance  float64
 81   PctJobs_ProductionTransportation                 float64
 82   OutageNumber                                     int64  
 83   OutageDuration                                   int64  
 84   NameplateCapacity_Total_MW                       float64
 85   NameplateCapacity_Wind_MW                        float64
 86   Pct_NameplateCapacity_Wind                       float64
 87   NameplateCapacity_SolarPV_MW                     float64
 88   Pct_NameplateCapacity_SolarPV                    float64
 89   NameplateCapacity_Batteries_MW                   float64
 90   Pct_NameplateCapacity_Batteries                  float64
 91   NameplateCapacity_LandfillGas_MW                 float64
 92   Pct_NameplateCapacity_LandfillGas                float64
 93   NameplateCapacity_NaturalGasCC_MW                float64
 94   Pct_NameplateCapacity_NaturalGasCC               float64
 95   NameplateCapacity_NaturalGasCT_MW                float64
 96   Pct_NameplateCapacity_NaturalGasCT               float64
 97   NameplateCapacity_NaturalGasST_MW                float64
 98   Pct_NameplateCapacity_NaturalGasST               float64
 99   NameplateCapacity_NaturalGasICE_MW               float64
 100  Pct_NameplateCapacity_NaturalGasICE              float64
 101  NameplateCapacity_PetroleumLiquids_MW            float64
 102  Pct_NameplateCapacity_PetroleumLiquids           float64
 103  NameplateCapacity_Coal_MW                        float64
 104  Pct_NameplateCapacity_Coal                       float64
 105  NameplateCapacity_Hydro_MW                       int64  
 106  Pct_NameplateCapacity_Hydro                      float64
 107  Oil_BBL_2022                                     float64
 108  Oil_Condensate_BBL_2022_TX                       float64
 109  Gas_Casinghead_MCF_2022_TX                       float64
 110  Gas_GW_MCF_2022_TX                               float64
 111  Gas_MCF_2022_NM                                  float64
 112  ElectricalPowerTransmissionLine_km               float64
 113  ElectricalPowerTransmissionLine_miles            float64
 114  CrudeOilPipeline_km                              float64
 115  CrudeOilPipeline_miles                           float64
 116  PetroleumPipeline_km                             float64
 117  PetroleumPipeline_miles                          float64
 118  NaturalGasPipeline_km                            float64
 119  NaturalGasPipeline_miles                         float64
 120  CO2Pipelines_km                                  float64
 121  CO2Pipelines_miles                               float64
 122  UtilityPV_TechPotential                          float64
 123  ResidentialPV_TechPotential                      float64
 124  CommercialPV_TechPotential                       float64
 125  LandbasedWind_TechPotential                      float64
 126  DistributedWind_TechPotential                    float64
 127  GeothermalHeatPump_EconPotential                 float64


Methodology
------------
1) Use Exploratory Data Analysis to determine which counties offer best opportunities to invest in renewable energy projects and type of project

2) Build correlation matrix and pair-plots to understand relationships between input variables

3) Supervised learning methods:
	a) Using linear regression to build a model that can explain what factors determine internet access in a county in the Permian basin
	b) Use Ridge regression and model pipeline method to improve model accuracy from step 3. Draw out MSE vs 1/alpha curves for training and development MSEs to find the optimum model parameters without over-fitting.
	c) Use Lasso regression to build model and compare model results with other methods


Expected Results
----------------
1) Counties identified in Texas most suitable for renewable energy projects based on their socio-economic data and existing oil and gas and renewable energy projects

2) Understand socio-economic factors that are conducive to investment opportunities in the renewable sector (wind and solar projects) in the Texas Permian basin

3) Understand socio-economic factors that determine the availability of internet access for workers in the Permian basin and how it may impact investment in renewable energy project


Why this question is important to me
------------------------------------
The U.S. economy is undergoing structural changes in the energy sector and there are vast opportunities to invest in renewable energy projects, especially in the Texas Permian Basin area. By analyzing NREL dataset on socio-economic status in the Permian Basin in Texas we can understand what factors drive opportunities in the wind and solar renewable energy projects and which countries in the Permian Basin in Texas are conducive for investment based on those factors. Investment right now in renewable energy can yield vast returns in both the short- and long-term for savvy investors. The goal of this report is to highlight such opportunities to those investors and potentially build a business case for investment.

Additionally, I work at ERCOT (www.ercot.com) that runs the electric grid in the state of Texas and understanding factors that drive renewable energy growth in the state can inform long-term planning for the grid.
