## Choosing a location for a well  

Let's say that the mining company GlavRosGosNeft has set the task of deciding where to drill a new well.  
We were provided with oil samples in three regions: in each 10,000 fields, where we measured the quality of oil and the volume of its reserves.  
We need to build a machine learning model that will help determine the region where mining will bring the greatest profit.  
Also, you need to analyze the possible profit and risks using the Bootstrap technique.  

# Steps to choose a location:  

- In the selected region, they are looking for deposits, for each, the values of the signs are determined;  
- Build a model and estimate the volume of reserves;  
- Select the deposits with the highest value estimates. The number of fields depends on the company's budget and the cost of developing one well;  
- The profit is equal to the total profit of the selected deposits.  

Data Description  

Geological exploration data of three regions are in the files:  

/datasets/geo_data_0.csv  
/datasets/geo_data_1.csv  
/datasets/geo_data_2.csv  

id - is the unique identifier of the well;  
f0, f1, f2 - three signs of points (it doesn't matter what they mean, but the signs themselves are significant);  
product is the volume of reserves in the well (thousand barrels).  

Conditions for completing the task:  
Only linear regression is suitable for training the model (the rest are not predictable enough).  
During the exploration of the region, 500 points are explored, from which, using machine learning, the best 200 are selected for development.  
The budget for the development of wells in the region is 10 billion rubles.  
At current prices, one barrel of raw materials brings 450 rubles of income.   
The income from each unit of the product is 450 thousand rubles, since the volume is indicated in thousands of barrels.  
After assessing the risks, you need to leave only those regions in which the probability of losses is less than 2.5%.  
Among them, choose the region with the highest average profit.  
Synthetic data: details of contracts and characteristics of deposits were not disclosed.
