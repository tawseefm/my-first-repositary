# my-first-repositary we will try to determine age group of verious people in this data set
## discreption - in this analysis we will determine marks of various age groups before pre test and post test in exam Jason','Molly','Tina','Jake','Amy' 
'age':[42,52,36,24,73],
## Getting Strated
## Dependencies
## Installing
## Executing program
#Load libraries
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
#Input some data
data ={'name':['Jason','Molly','Tina','Jake','Amy'],
      'age':[42,52,36,24,73],
      'preTestScore':[4,24,31,2,3],
      'postTestScore':[25,94,57,62,70]}
 {'name': ['Jason', 'Molly', 'Tina', 'Jake', 'Amy'],
 'age': [42, 52, 36, 24, 73],
 'preTestScore': [4, 24, 31, 2, 3],
 'postTestScore': [25, 94, 57, 62, 70]}
 ## Convert Data into a Dataframe
df=pd.DataFrame(data, columns =['name','age','preTestScore','postTestScore'])
df.head()
name	age	preTestScore	postTestScore
0	Jason	42	4	25
1	Molly	52	24	94
2	Tina	36	31	57
3	Jake	24	2	62
4	Amy	73	3	70
# Show "name" variable
df['name']
0    Jason
1    Molly
2     Tina
3     Jake
4      Amy
Name: name, dtype: object
# Show "age" variable
df['age']
0    42
1    52
2    36
3    24
4    73
Name: age, dtype: int64
## Transpose Dataframe
df.T
	0	1	2	3	4
name	Jason	Molly	Tina	Jake	Amy
age	42	52	36	24	73
preTestScore	4	24	31	2	3
postTestScore	25	94	57	62	70
#Create Simple Line Graphs

## Plot Lines
plt.plot(df.preTestScore, label='preTestScore')
plt.plot(df.postTestScore, label='postTestScore')

## Titles
plt.title('Test Score Results')
plt.xlabel('Name')
plt.ylabel('Score')

## Legend 
plt.legend(bbox_to_anchor=(1.05, 1), loc=2)
plt.show()
# Help
# Authors
@tawseefm
## Version History
0.1
initial release 
## License
This project is licensed under the [Tawseef Mir] License - see the LICENSE.md file for details
