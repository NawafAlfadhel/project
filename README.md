# project
#project python
# الهدف:هو تحليل البيانات بشكل بسيط و تفسيرها باستخدام لغةبرمجة (بايثون)



# تم العمل على بيانات وتم الحصول على التالي :
#متوسط سعر الايتم
#السعر الاعلى و الاقل 
# var للكمية
#السعر في الكمية للحصول على المبيعات في تاريخ المعين 
# تم عمل التكرار في مناطق لمعرفة اكثر منطقه تم البيع فيها 
# تم عمل التكرار في اسم البائع لمعرفه اكثر شخص سوق اوباع 
# و تم العمل التكرار على التاريخ لمعرفة اكثر يوم تم البيع فيه

import pandas as pd 
df=pd.read_csv('bayan.csv')
df
df['Price'].mean()
df['Price'].max()
df['Price'].min()
df['Quantity'].var()
df['Quantity'].count()
df['Quantity'].sum()
df['Quantity']*df['Price']
df['Quantity']/df['Price']
df['Quantity']+df['Price']
df['Region'].value_counts()
df['Sales Person'].value_counts()
df['Customer Name'].value_counts()
df['Date'].value_counts()
