# World-Bank-Data-Cleanup
___
**Contributor** : Francis Mangala

**Coding Languages** : Python Pandas

**Description** : This code is too clean up aggregates ,regions, and country names. 

**The country raw data set from has country group aggregates such as**: 
* South Asia (IDA & IBRD), 
* Early-Demographic dividend, 
* Fragile and conflict affected situations, 
* Upper World, etc.

**also country names that are different from the standards such as**:

* Congo,Dem.Rep -> of Democratic Republic of Congo; 
* Korea,Dem. People -> North Korea; 
* Syrian Arab Republic -> Syria
* etc,

With one click, this code allows you to delete all the country group aggregates, and modify the country names to meet the standards. Then, it will merge the regions files, and re-order all the columns to have a clean dataset.

## To pivot the table you can use this code : 
___
```
pivot_df = pd.melt(df_1,id_vars=['Country Name','Country Code','IncomeGroup'],
value_vars=['1960','1961', '1962', '1963', '1964', '1965', '1966', '1967', '1968', '1969', '1970',
'1971','1972', '1973', '1974', '1975', '1976', '1977', '1978', '1979', '1980', '1981', '1982', '1983', '1984', '1985', '1986',
'1987', '1988',  '1989', '1990', '1991', '1992', '1993', '1994', '1995', '1996', '1997', '1998', '1999', '2000', '2001', '2002',
'2003', '2004', '2005', '2006', '2007', '2008', '2009', '2010', '2011', '2012', '2013', '2014', '2015', '2016', '2017', '2018',
'2019', '2020', '2021'],var_name='Year')
pivot_df
```
___
#### 1) The first step is to open the raw data file, delete the first 3 rows so that the country name cell is on A1, and then save it.(See picture of the raw country data file below).
![image](https://user-images.githubusercontent.com/78506782/208540959-1567a1ed-0c84-4997-a035-afd06ed4ef23.png)
#### 2) Below is a snapshot of the raw region data file
![image](https://user-images.githubusercontent.com/78506782/208546926-55716af7-d355-4195-89a9-98daec15300c.png)

#### 3) After merging both files, the code export a clean csv dataset with dates ranging from 1960 -2021.( See picture below)

![image](https://user-images.githubusercontent.com/78506782/208547419-812d8d85-a86f-44c2-8963-2ec4ed686db4.png)


