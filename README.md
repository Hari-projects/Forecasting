# Forecasting

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
<html lang="en" style="width:100%; height:100%;">
<head>
  <meta http-equiv="content-type" content="text/html; charset=utf-8">
  <title>Buxton Challenge</title>
</head>
  <body style="width:100%; height:100%; margin:0;">
    <iframe src="https://docs.google.com/gview?url=  https://github.com/Hari-projects/Academic-Projects/blob/master/Forecasting &embedded=true" style="width:100%; height:100%;" frameborder="0"></iframe>
  </body>
</html>


Executive Summary

The client, Jen’s Gem Gym (JGG) is a fitness club for those that want to polish every facet of their abilities to really shine. Looking to expand its operations, the client has 20 potential locations under consideration.

Relying on guidance from the literature and data analysis techniques, we developed a sales forecasting model to aid the identification of new locations with strong revenue potential.

Based on the predicted sales performance for each location, we identified a total of 6 potential locations that the client should consider as a new JGG location. The recommended locations are presented in the table below.

 

Table Showing Recommended New JGG Locations


 
Introduction

The client, Jen’s Gem Gym (JGG) is a fitness club for those that want to polish every facet of their abilities to really shine. With the executive leadership running out of easy win locations following a period of successful, aggressive expansion, the client is looking to switch from its aggressive expansion strategy to a more conservative approach.

The client has 20 locations under consideration and is looking to us to develop a sales forecasting model to aid the identification of new locations with strong revenue potential. The next section provides an overview of the gym and fitness industry where JGG operates.

Industry Overview

With profits of $3.8bn from overall industry revenues of $33.4bn in 2018, according to an IBISWorld 2018 report, the fitness industry in the United States has done quite well for itself in recent years. Although growth is projected to slow to 1.1% between 2018 and 2023, from a decent 2.6% growth rate recorded between 2013 and 2018, the overall prospects of the industry remain bright. As consumer disposable incomes and desire for healthier lifestyles increase, the fitness industry is projected to continue to grow for the foreseeable future. The next section discusses some of the key drivers of revenues for gyms in the USA.

Key Revenue Drivers

1.	Per capita disposable incomes - According to the IBISWorld 2018 report, as per capita disposable income rise, due to favorable changes in government policies and economic conditions, more individuals will be able to purchase fitness club memberships. More customers would also be able to afford relatively high-cost memberships that offer more benefits.

2.	Number of Adults Aged 20 to 64 - According to IBISWorld, individuals aged 20 to 64 make up the largest gym-going demographic.












Figure 1: Fitness Industry Market Segmentation by Age

The traditional market of 18- to 35-year-olds constitute the chunk of the overall market at 27% and are predicted continue to be the largest segment for the foreseeable future. Individuals aged 35 to 50, make up the next largest segment with 27%, but this segment is predicted to remain stagnant for the foreseeable future. In terms of growth prospects, the most exciting segments are those aged 21 and younger and the segment for customers age 50 and above. These segments are projected to grow rapidly due to an increase in health consciousness (to combat the deleterious effects of inactivity and obesity on health) and also due to an increase in the number of gyms offering programs that are targeted specifically towards these segments.

3.	Leisure Time Availability and Attitudes towards Health and Fitness - The amount of time individuals have available for leisure activities is another factor that influences demand for gym memberships. Painting with broad strokes, the individuals or market segments that have greater leisure time available are more likely to incorporate fitness activities into their routine. Similarly, as more and more people and businesses embrace the proven health benefits of regular exercise, more and more individuals are predicted to join gyms and fitness clubs.

4.	Location Accessibility - Another factor that impacts revenue for gym and fitness club is ease of access to the location for the target market. According to Marlin Dean, a fitness industry consultant, a gym should be situated no more than a 12-minute drive from its target market. He also recommends situating a gym on high visibility roads and in close proximity to convenience retail favored by the target market as this ensures the gym is located along the target market’s routine driving routes.

5.	Competitors - In an article published by Precor, a fitness services provider, it is important for a new gym to consider which competitors are in the trade area, which market segment they target, and the potential impact of these competitors on revenues. 

 
The Client

Jem’s Gem Gym (JGG), a fitness club with over 500 locations across the US is looking to identify new locations with strong revenue potential.

Jem’s Gem Gym currently has 547 locations spread across 44 states in the USA. The figure below shows the current distribution of location(s) per state where JGG has a presence.































Table 1: Number of JGG Locations by State




In line with national trends, JGG has 77 locations (or 14.08% of its total number of locations) in Florida, 66 locations (12.07%) in California, and 50 locations (9.14%) in Texas.

In terms of sales performance, JGG generated a total of $2.67 billion in revenue from its 547 operational locations, with California, Florida and Texas the top-performing states. The table below reports the average sales performance per state, highest and lowest sales, and overall total sales revenue for 2018.

Table 2: JGG Sales Performance by State 
Table 2: JGG Sales Performance by State (contd)

With 20 potential locations under consideration, JGG is looking to identify new locations with strong revenue potential in line with its expansion strategy. Under consideration are 4 potential locations each in California and Texas, 3 potential locations each in Colorado and Indiana, and 1 location each in Florida, Georgia, Michigan, Ohio, South Carolina, and Utah.

The next section details the methodology we adopted in building a sales forecasting model to predict sales revenue for the locations under consideration.

 
Model Building Methodology

Our first stop in our model building approach was to consult the literature to identify those factors that are the key predictors of sales performance for a gym or fitness club. Through a search of the literature and secondary data sources, we identified factors such as disposable income, number of adults age 20 to 64, location accessibility, etc. which have already been discussed in detail in previous sections.

Due to the strong influence that location accessibility has on gym/fitness club revenues, we decided to largely focus on variables at the 9-minute drive level in our model building efforts.

Guided by the literature, intuition, and our interaction with the data, we identified 11 variables as being the best predictors of sales revenue for the potential new locations. The table below presents the selected/identified variables.

 

Table 3: Variables in Sales Forecasting Model
 
The table below presents the summary statistics for the variables.

 

Table 4: Descriptive Statistics for Model Variables


Sales Forecast Model

Our sales forecast model is a linear regression model which has sales as the dependent variable and the variables above as the independent variables. Formally the model is described by the equation;


SALES = ᵦ0 + ᵦ1 AGE_ADULT18P_9TO + ᵦ2 CMDSC_COMP_B_1RO + ᵦ3 HH_9TO + ᵦ4 COMMUTE_AVG_9TO + ᵦ5 HHSZ_AVG_9TO + ᵦ6 POCHH_2RO + ᵦ7 POPGROW5YR_9TO + ᵦ8POPGROWSINCE2010_9TO + ᵦ9 VEH_AVG_18TO + ᵦ10HHINC_MED_COLADJ_9TO + ᵦ11POP_9TO
 
The table below presents the Stata output for the linear regression model.
 
Table 5: Stata Output for Sales Forecasting Model

To address the issues of heteroscedasticity in our data, we log-transformed the variables and re-ran the model in Stata. We also made sure to further correct for heteroscedasticity by requesting for robust standard errors. The output with the log-transformed variables is shown below.
 
Table 6: Stata Output for Sales Forecasting Model with Log Transformed Variables
Sales Revenue Prediction
Using the model above, we predicted the sales for the 20 potential locations under consideration. The predicted sales for the top five locations are presented in the table below. 
 
Table 7: Predicted Sales for Potential Sales Locations

 
Conclusion and Recommendations
The table below compares the predicted sales revenue for each potential location with the average sales revenue for each state, and based on this comparison, we recommend JGG opens a new gym at each location that is predicted to outperform the state average (locations highlighted in the table below). In summary, we recommend that JGG strongly consider opening new gyms in each of the 6 locations highlighted below.
 
Table 8: Predicted Sales Revenue for Potential Sales Locations Compared to State Averages (recommended locations are highlighted)
	

 
References 
1.	"11 Things New Gym Owners Should Consider When Opening A Fitness Club." LinkedIn. Accessed April 20, 2019. https://www.linkedin.com/pulse/11-things-new-gym-owners-should-consider-when-opening-marlin-dean.

2.	How to Choose a Location for Your New Gym." How to Choose a Location for Your New Gym - Precor (US). Accessed April 20, 2019. https://www.precor.com/en-us/resources/how-choose-location-your-new-gym.

3.	IBISWorld Industry Report 71394 Gym, Health & Fitness Clubs in the US, December 2018

4.	Lake, Rebecca. "23 Gym Membership Statistics That Will Astound You." CreditDonkey. Accessed April 20, 2019. https://www.creditdonkey.com/gym-membership-statistics.html.

5.	Moretti, Lawrence. "Location Strategy Decision Chain | Supply (and Demand) Decision Chain." Area Development. May 15, 2009. Accessed April 20, 2019. 

6.	http://www.areadevelopment.com/siteSelection/Apr09/location-stragegy-decision-chain001.shtml.

7.	Riggins, Nash. "How to Start Your Own Gym." Small Business Trends. August 23, 2016. Accessed April 20, 2019. https://smallbiztrends.com/2016/08/how-to-start-your-own-gym.html.
 
Stata Do Files
C:\Users\Kathy\Documents\Spring 2019\econ5339\Buxton\gym2.dta clear
reg sales age_adult18p_9to cmdsc_comp_b_1ro hh_9to commute_avg_9to hhsz_avg_9to pochh_2ro popgrow5yr_9to popgrowsince2010_9to veh_avg_18to hhinc_med_coladj_9to pop_9to
* to compare yvariable between two xvariables
ipolate sales age_adult18p_9to , gen(newsales2) epolate by ( state )
br
* testing prediction
predict sales_predict if e(sample)
predict sales_resid, res
reg sales age_adult18p_9to cmdsc_comp_b_1ro hh_9to mpop_9to pochh_2ro popgrow5yr_9to popgrowsince2010_9to race_asiapop_9to hhinc_med_coladj_9to
*log variables*
gen lnsales = ln(sales)
gen lncmd = ln( cmdsc_comp_b_1ro)
gen lncomm = ln( commute_avg_9to )
gen lnhhinc = ln( hhinc_med_coladj_9to)
gen lnhhsz = ln( hhsz_avg_9to )
gen lnhh_9to = ln( hh_9to)
gen lnpochh_2ro = ln( pochh_2ro)
gen lnpopgo5yr = ln( popgrow5yr_9to )
gen lnpopgrow2010 = ln( popgrowsince2010_9to)
reg lnsales age_adult18p_9to cmdsc_comp_b_1ro commute_avg_9to lnhhinc hhsz_avg_9to hh_9to pochh_2ro popgrow5yr_9to popgrowsince2010_9to pop_9to veh_avg_18to, r
