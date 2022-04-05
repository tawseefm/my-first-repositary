# my-first-repositary 
we will try to determine the pre marks and post marks of various age group of verious people in this data set
## discreption 
in this analysis we will determine marks of various age groups before pre test and post test in exam Jason','Molly','Tina','Jake','Amy' 
'age':[42,52,36,24,73],
## Getting Strated
## Dependencies
Pandas,numpy,matplotlib
## Executing program
#Load libraries<br>

import pandas as pd<br>

import matplotlib.pyplot as plt<br>
%matplotlib inline<br>
#Input some data<br>

data ={'name':['Jason','Molly','Tina','Jake','Amy'],
      'age':[42,52,36,24,73],
      'preTestScore':[4,24,31,2,3],
      'postTestScore':[25,94,57,62,70]}<br>
      
 {'name': ['Jason', 'Molly', 'Tina', 'Jake', 'Amy'],<br>
 'age': [42, 52, 36, 24, 73],<br>
 
 'preTestScore': [4, 24, 31, 2, 3],<br>
 
 'postTestScore': [25, 94, 57, 62, 70]}<br>
 
 #Convert Data into a Dataframe<br>
 
df=pd.DataFrame(data, columns =['name','age','preTestScore','postTestScore'])<br>
df.head()<br>

#Show "name" variable<br>
df['name']<br>

Name: name, dtype: object<br>

#Show "age" variable<br>
df['age']<br>

Name: age, dtype: int64<br>

#Transpose Dataframe<br>
df.T<br>

#Create Simple Line Graphs<br>

#Plot Lines<br>
plt.plot(df.preTestScore, label='preTestScore')<br>
plt.plot(df.postTestScore, label='postTestScore')<br>

#Titles<br>
plt.title('Test Score Results')<br>
plt.xlabel('Name')<br>
plt.ylabel('Score')<br>

#Legend <br>
plt.legend(bbox_to_anchor=(1.05, 1), loc=2)<br>
plt.show()<br>
## Authors
@tawseefm

## Version History
0.1
initial release 

## License
This project is licensed under the [Tawseef Mir] License - see the LICENSE.md file for details
