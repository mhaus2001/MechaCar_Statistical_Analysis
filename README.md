# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
[Linear_Data.png](https://github.com/mhaus2001/MechaCar_Statistical_Analysis/blob/main/Starter_Code/Photos/Linear_Data.png)
This linear regression was made to predict the mpg of MechaCar prototypes using several variables from the `MechaCar_mpg.csv`file
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  - The Vehicle length with p-value=2.60e-12 which is « 0.05 and vehicle ground with p-value=5.21e-08 which is « 0.05 clearance are shown in the summary that statistacally they are likely to provide a non-random amount of variance.
- Is the slope of the linear model considered to be zero? Why or why not?
  - The slope is not considered to be zero as the p-value(5.35e-11)is smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject the null hypothesis.
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  - Consdering the R value of 0.7149 it shows that a majority of the data can be predicted from the model that has been constructed, as such while there can be improvements made to the model to improve its predictive ability it does prove sufficently effective for its given task.
## Summary Statistics on Suspension Coils
[Total_sum.png](https://github.com/mhaus2001/MechaCar_Statistical_Analysis/blob/main/Starter_Code/Photos/Total_Sum.png)
[Lot_Sum.png](https://github.com/mhaus2001/MechaCar_Statistical_Analysis/blob/main/Starter_Code/Photos/Lot_Sum.png)
The above images contain the sumamry data from the Suspension_Coil.csv dataset pertaining to the information on the weight capacities of multiple suspension coils that  were tested to determine if the manufacturing process is consistent across the production lots
- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
  - The lots summarised, as shown in the above images, all meet the specifications of having varience that does not exceed 100 pounds per square inch, with the exception of lot 3 that has a variance(170) that is signifigantly higher than that of the desired specifications. As such the current manufaturing data only mostly meets the current specifcations.
## T-Tests on Suspension Coils
[T_test_1.png](https://github.com/mhaus2001/MechaCar_Statistical_Analysis/blob/main/Starter_Code/Photos/T_test_1.png)
[T_test_2.png](https://github.com/mhaus2001/MechaCar_Statistical_Analysis/blob/main/Starter_Code/Photos/T_test_2.png)
[T_test_3.png](https://github.com/mhaus2001/MechaCar_Statistical_Analysis/blob/main/Starter_Code/Photos/T_test_3.png)
I preformed t-tests using R to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch. In the tests conducted only lot 3 showed statistical differences, as seen in the above photos, this is supported by the difference shown in previous data with variance being signifigantly different from the other lots.
## Study Design: MechaCar vs Competition
I designed a statistical study to compare performance of the MechaCar vehicles against performance of competitors with details of the study being shown below
- What metric or metrics are you going to test?
  - The metric that is going to be tested in this study is the saftey rating and as well vehicle wieght
- What is the null hypothesis or alternative hypothesis?
  - The null hypothesis is: Heavier cars are no safer than lighter cars
- What statistical test would you use to test the hypothesis? And why?
  - The test I would use is a Chi-Squared Test as this test can determine if there is a difference in categorical frequencies between groups such as, what number of  vehicles in wieght category A have a safety rating of B? vs. what number of vehicles in weight category B have a safety rating of B?
  - it also allow us to reject the null hypothesis if the pvalue is below .005 in the test providing answer to rether vehicle wieght affects saftey rating 
- What data is needed to run the statistical test?
  - Vehicle weight data for Mechacars and as well competiors and as well crash data for all cars so as to be able to preform the study allowing for comparsion of the mechacars models and competitors 
