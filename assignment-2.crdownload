#!/usr/bin/env python
# coding: utf-8

# In[7]:


import numpy as np


# In[8]:


a=np.random.randint(1,20,15)


# In[9]:


a=a.reshape(3,5)
a


# In[10]:


a.shape


# In[11]:


a[np.isin(a, np.max(a,axis=1))]=0
a


# In[131]:


import pandas as pd


# In[74]:


df=pd.read_csv("./data.csv")


# In[75]:


mean_value=df['Calories'].mean()


# In[76]:


df['Calories'].fillna(value=mean_value,inplace=True)


# In[44]:


df.head(25)


# In[45]:


df.Duration.describe()


# In[46]:


df.Pulse.describe()


# In[47]:


df[(df['Calories']>500) & (df['Calories']<1000)]


# In[48]:


df[(df['Calories']>500 & (df['Pulse']<100))]


# In[49]:


df_modified=df.drop("Maxpulse",axis=1)


# In[50]:


df_modified


# In[77]:


df=df.drop("Maxpulse",axis=1)


# In[52]:


df


# In[78]:


df['Calories']=df['Calories'].astype(int)


# In[79]:


df.dtypes


# In[59]:


df.plot.scatter( x = 'Duration', y = 'Calories')


# 3. Matplotlib
# 1. Write a Python programming to create a below chart of the popularity of programming Languages.
# 2. Sample data:
# Programming languages: Java, Python, PHP, JavaScript, C#, C++
# Popularity: 22.2, 17.6, 8.8, 8, 7.7, 6.7

# In[46]:


prgmng_df=pd.DataFrame({"popularity":[22.2, 17.6, 8.8, 8, 7.7, 6.7]},index=['Java','Python','PHP','JavaScript', 'C#', 'C++'])
prgmng_df


# In[48]:


prgmng_df.plot.pie(y='popularity',autopct='%1.1f%%')

