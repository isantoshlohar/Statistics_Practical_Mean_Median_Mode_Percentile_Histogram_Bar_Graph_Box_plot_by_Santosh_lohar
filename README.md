####---Import---Python----library-----####
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
%matplotlib inline
####---Import---statistics---library--####
import statistics
####---Import---dataset-----####
df=sns.load_dataset('tips')
df.head()
** dataset **
total_bill	tip	sex	smoker	day	time	size
0	16.99	1.01	Female	No	Sun	Dinner	2
1	10.34	1.66	Male	No	Sun	Dinner	3
2	21.01	3.50	Male	No	Sun	Dinner	3
3	23.68	3.31	Male	No	Sun	Dinner	2
4	24.59	3.61	Female	No	Sun	Dinner	4
**
####---find-----mean-----####
sns.mean(df['total_bill'])

####---find-----median-----####
sns.median(df['total_bill'])

####---find-----mode-----####
statistics.mode(df['total_bill'])

####---find---boxplot-----####
sns.boxplot(df['total_bill'])

####---find---histogram-----####
sns.histplot(df['total_bill'],kde='true')

####---find---percentile-----####
np.percentile(df1['sepal_length'],[25,75])











