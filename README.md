# Drug Tumor effect analysis on Mouse subjects - Matplotlib
This module applies data visualisation with research statistic on mouse test subjects, where each has been dosed with different drugs. The results contains stats that measures the tumor volume, the amount of drugs dosed onto the specimen and the age of the mouse. These results has been used to create various visual graphs which showcase unique information, trends and insights that a dataframe couldn't show. <br/>

## Development Process
The data file contains two csv files; **mouse metadata path & Study Results**. These datas were merged into Table on the Mouse ID as well as removing any duplicate that was found in the dataset, the final table was shown below: <br/>
![image](https://github.com/EricTran99/Assignment-5-Drug-ploting/assets/134130254/13ce7638-755d-43e3-bb70-82221e8cca9e) <br/>
 <br/>
With the cleaned dataset, the tumor volume value was used to calculate the summary statistics (_mean, median, variance, standard deviation, SEM_) for each drug regimens. Two methods were used to perform the calculation; the first hard calculates the volumes with the scipy package. Whereas the second method applied the **aggregate** command and group the results with the drug regimens. The dataset was shown below: <br/>
![image](https://github.com/EricTran99/Assignment-5-Drug-ploting/assets/134130254/490789aa-9bef-49f8-a5da-1302c06ec7b6) <br/>
 <br/>

## Data Visualisation & Observations
The first data visualisation was a **bar graph**, the graph below is the total number of mouse specimens timepoint per drugs. The observation shows that _Propriva_ has less survived mouse than mouse specimens that were dosed with _Capomulin_ & _Ramicane_. One reason could be that it is more lethal and so some of the mouse test subject hasn’t survived the full duration of the test. However, there may be a possibility that the drug has removed the tumour. However, this highlights which drugs would be focused onto for further results. <br/>
![image](https://github.com/EricTran99/Assignment-5-Drug-ploting/assets/134130254/a99d8f90-effc-493f-ad4c-f34450765a38) <br/>
 <br/>
Since _Capomulin_ had the highest number of survived mouse specimens, that specific drug's results was used to create a **Line graph** which display the Tumor volume across the Timepoints. What the graph showed was a change in Tumor volume within the 20 days where the drug had impacted the Tumor, causing it to shrink according to the results (which supports the reason why mouse dosed with _Capomulin_ survived based on the bar graph). However, after 30 days, the Tumor grew in size, indicating the drug dose amount isn't enough to stop the tumor. <br/>
![image](https://github.com/EricTran99/Assignment-5-Drug-ploting/assets/134130254/fd2201bc-5e6b-4b3a-a44a-1a1c87fb48ec) <br/>
 <br/>
The third visual graph was a **scatter plot** with the Average Tumor Volume by the mouse weigh. The scatterplot showcased a relatively straight line, with the line annotated and the value of 0.84 supporting the claim. This means that the tumour size does have some dependency on the mouse’s weight. One possible reasoning may be that the increasing weight lead to higher mass, which in turn means the tumour size grows as with the increased resource for growth.
![image](https://github.com/EricTran99/Assignment-5-Drug-ploting/assets/134130254/463fd4a0-2d7c-41e0-8748-ead3a51645f5) <br/>
 <br/>
# Summary
The focus of the data was to extract the results and convert the dataset by cleaning and removing duplicate, which would be used to create various visual graphs that support the specific drug that could be used to neutralise the tumor growth. The graphs supports the statements upon the tumor's properties based on the subject's weight, in addition that _Capomulin_ showed to be the most effective drug among the other regimens.
