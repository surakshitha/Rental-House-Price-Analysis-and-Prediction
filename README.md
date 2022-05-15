<div style="text-align: justify;"><h1 style="text-align: centre !important;">CS649 Big Data Analytics Project</h1>
<h3>Objective of project:</h3><br>
<ul>
<li><em><u><b>Predictive Analysis:</b></u></em> To model a dataset of house rental prices using various machine learning algorithms to predict rental prices depending on multiple explanatory variables that describe the elements of the residential property.<br>  
<u><b>Exploratory analysis:</b></u> Summarize the main characteristics and analyze the dependencies between the variables and the rental prices using statistical graphs and visualizations.<br>
<u><b>Comparative Analysis:</b></u> Compare the machine learning algorithms and their performance.</li>
<br>
<li><em><u><b>Dataset description:</b></u></em> rentalHousing.csv This file contains rental house listings from Craigslist for south eastern regions between San Francisco bay area and San diego. This includes all information regarding the rental listing which includes url of the listing, region of the property, area(sqft.), number of baths and beds, cats and dogs allowed, wheelchair accessibility, electric charging point availability for vehicles, laundry options, smoking permission, description of the property, location (latitude & longitude) and etc. We have about 18300 records consisting of thirteen numerical features and nine categorical features.</li>
<br>
<li><em><u><b>Tech and libraries:</b></u></em> We have implemented the project using both pandas and Spark pandas separately. The Spark pandas version runs smoothly on Spark 3.2.1 and Jupyter. You are required to run the second cell in this notebook to set up all the necessary environment variables and import the required libraries. Due to efficiency and lesser running time, we are submitting the pandas version of the project application. For running the pandas version of the project, which is this notebook, we will requrie XGBoostRegressor library to be installed.</li>
 <br>
<li><b><em><u>Issues and challenges:</u></em></b>
<ul>
With spark pandas version:<br><ol><li>We had to resolve dtype conflicts and convert our data to numpy ndarray or a pandas dataframe to successfully visualize & fit data into models.</li>
<li>The main issue we faced was memory. The main reason being, the entire RAM was used up and the session times out. We resolved this issue by increasing the value of spark.driver.memory to 15gb in the spark-defaults.conf configuration file.</li>
<li>We need to plot the graphs using pandas DataFrame since Spark does not having functions to plot graphs.</li><ol></li>
<ul>
</li>
</ul> 
    </div>
