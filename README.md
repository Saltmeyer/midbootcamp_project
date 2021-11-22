https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png

PROJECT TITLE
Correlations among weather and electricity prices in Spain.

PROJECT DESCRIPTION
This project was the mid-bootcamp project, part of the Ironhack Data Analysis bootcamp in November 2021 after four weeks of lessons. 

This project uses energy markets and weather data from Spain to examine correlations of wholesale electricity market prices in Spain. The analysis uses two datasets  which provide hourly data on selected weather variables as well as 
electricity prices and source generation data from 2015 and 2018. Both datasets were retrieved via kaggle.com (see credits). The goal of the project is to examine the influence of the selected weather variables on wholesale electricity 
market prices. In particular, the project aims to examine if weather conditions suitable for electricity generation from wind and solar can lower wholesale electricity prices. Due to technological advances, the levelised cost of
electricity (marginal cost to produce electricity) of wind and solar technologies have fallen significantly over the past years. Therefore, a growing share of wind and solar could lower electricity prices if weather conditions are
favourable. It should be added that there are limitations, as the regulatory framework might affect prices building as well. Naturally, weather has an influence on electricity prices outside the spheres of renewable energy generation.
As Spain enjoys warm to hot summers, air conditioning is commonly used in the summer months, which requires a lot of electricity. This is shown in the analysis. Temperature has a positive correlation with electricity prices.

The weather dataset contains hourly weather data for the five largest five cities in Spain - Madrid, Bilbao, Barcelona, Valencia and Seville. These cities roughly represent  various cardinal points in Spain. Thus, the analysis is build
on the assumption that an average of these five cities roughly represents the weather for Spain as a whole. The weather data is grouped to show the average of those variables for every time point.

After general cleaning, an exploratory analysis examines the data, in particular distributions and bivariate correlation analysis and plotting. Chi contingency hypothesis testing is used to identify correlations of the weather variables
temperature, wind_speed and cloud cover. Finally, a simple machine learning model is build to see if the weather data may be used to predict electricity prices. As the shares of wind and solar energy are still relatively low, it was
not expected that electricity prices could be precisley predicted. Rather, the model was created to show that already a small share of renewable energy have some significant influence and this influence may increase in the future.

The project contains five data files. Principal cleaned data is stored in weather_data.csv and energy_data.csv. For the analysis, the file weather_eprice.csv contains selected weather variables and the electricity prices, sliced from
energy_data.csv. The files main_data , energy_tableau.csv ,  energy_tab5.csv , energy_grouped.csv and energy_grouped_2.csv were created for Tableau to create graphs suitable for the presentation.


SOFTWARE USED
This analysis uses Python via Jupyter Notebook for the statistical analysis. Data is stored in MySQL. Tableau Public is used to create graphs and a story for the project's presentation.

ACCESS TO MATERIAL

Github: 

Tableau story: https://public.tableau.com/app/profile/severin.altmeyer/viz/Presentation_Midtermproject_Ironhack/WeatherElectricity?publish=yes

Project Use
Others are welcome to expand and build on the work already done. The pre-cleaned data can be used to examine further correlations or expand the analysis to all four years of weather and energy data.

Credits
Both datasets were downloaded from kaggle.com and provided by Nicholas Jhana.

https://www.kaggle.com/nicholasjhana/energy-consumption-generation-prices-and-weather

"This dataset contains 4 years of electrical consumption, generation, pricing, and weather data for Spain. Consumption and generation data was retrieved from ENTSOE a public portal for Transmission Service Operator (TSO) data. 
Settlement prices were obtained from the Spanish TSO Red Electric España. Weather data was purchased as part of a personal project from the Open Weather API for the 5 largest cities in Spain and made public her



List the License
Copyright (c) [2021] [Severin Altmeyer]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
