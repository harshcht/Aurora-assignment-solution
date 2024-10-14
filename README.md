# Aurora-assignment-solution

Solution summary : 
The solution optimises a revenue / cost function formed by summing up the revenue in each 30 min block throughout the time period. Solving the problem for all three  in one single go  proves to be computationally expensive and thus the problem is divided into days, and the solution of each day is summed up to give the final solution at the end. The limit on number of battery cycles and reduction in battery capacity with battery capacity is modelled by calculating the total energy exchanged by the battery (calculated by summing the absolute values of energy charge/discharge).
Therecan be two interpretations of the way in which power is traded simultaneously.  In the first interpretation, more power thanthe battery’s limit can be traded in total if extra power is purchased from theother one. For example, for a 2MW battery, 2MW can be sold into each market 1and 2 and 2 MW can be bought from market 3. In the second interpretation such operation is not allowed. The solution for the second solution is suboptimal. 
 
File descriptions  :   

The model assumptions and limitations are described in solution.pdf  
the excel  files   (solution1.xlsx and solution2.xlsx) have two sheets each : schedule (describing the half hourly schedule (-ve for charging and +ve for discharging)). and revenue (showing annual revenue and operational profits). Each excel file gives the solution for each interpretation. 

On running the jupyter notebook (daily.ipynb) it generates a test.csv, containing the schedule for each market and the total battery charge/ discharge. Its data can be copied into columns E to H in solution file to get the annual revenue and profits. 