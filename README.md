# World-Bank-Data-Cleanup
#### Contributor : 
Francis Mangala
#### Languages : 
Python Pandas
#### Description : 

This code is too clean up aggregates ,regions, and country names. 
The country raw data set from has country group aggregates such as: 
#### South Asia (IDA & IBRD), Early-Demographic dividend, Fragile and conflict affected situations, Upper World, etc.
also country names that are different from the standards such as: 
#### Congo,Dem.Rep -> of Democratic Republic of Congo; 
#### Korea,Dem. People -> North Korea; 
#### Syrian Arab Republic -> Syria
#### etc,

With one click, this code allows you to delete all the country group aggregates, and modify the country names to meet the standards. Then, it will merge the regions files, and re-order all the columns to have a clean dataset.

#### 1) The first step is to open the raw data file, delete the first 3 rows so that the country name cell is on A1, and then save it.(See picture of the raw country data file below).
![image](https://user-images.githubusercontent.com/78506782/208540959-1567a1ed-0c84-4997-a035-afd06ed4ef23.png)
#### 2) Below is a snapshot of the raw region data file
![image](https://user-images.githubusercontent.com/78506782/208546926-55716af7-d355-4195-89a9-98daec15300c.png)

#### 3) After merging both files, the code export a clean csv dataset with dates ranging from 1960 -2021.( See picture below)

![image](https://user-images.githubusercontent.com/78506782/208547419-812d8d85-a86f-44c2-8963-2ec4ed686db4.png)


