# exam
import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv("matcars.csv")
x=df.wt
y=df.mpg
plt.xlabel('Weight')
plt.ylabel('Mpg')
plt.scatter(x,y)
plt.title('scatter plot')
plt.show()

a=df.hp
b=df.vs
plt.xlabel('hp')
plt.ylabel('vs')
plt.bar(a,b,color ='green',edgecolor='blue',linewidth=6 )
plt.title('barplot')
plt.show()

y= df.mpg
plt.hist(y,   bins = 5 ,);
plt.title('histogram')
plt.show()

sns.boxplot(df['hp'])
plt.title('box plot and whisker')
plt.show()
