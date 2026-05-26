# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
~~~
 import matplotlib.pyplot as plt
import pandas as pd
from sklearn.datasets import load_iris

# STEP 1: Load dataset
iris = load_iris()

# STEP 2: Convert to DataFrame
df = pd.DataFrame(
   iris.data,
   columns=iris.feature_names
)
~~~
~~~
# STEP 3: Visualize data

# Line Plot
plt.figure(figsize=(6,4))
plt.plot(df["sepal length (cm)"])
plt.title("Line Plot")
plt.xlabel("Index")
plt.ylabel("Sepal Length")
plt.show()
~~~

<img width="694" height="394" alt="image" src="https://github.com/user-attachments/assets/d42343d1-d131-44ea-8be8-df3805aa465c" />

~~~
# Histogram
plt.figure(figsize=(6,4))
plt.hist(df["petal length (cm)"], bins=10)
plt.title("Histogram")
plt.xlabel("Petal Length")
plt.ylabel("Frequency")
plt.show()
~~~

<img width="605" height="392" alt="image" src="https://github.com/user-attachments/assets/06249598-c43d-4204-b5ae-73c79adbc5f3" />

~~~

# Scatter Plot
plt.figure(figsize=(6,4))
plt.scatter(
    df["sepal length (cm)"],
    df["petal length (cm)"]
)
plt.title("Scatter Plot")
plt.xlabel("Sepal Length")
plt.ylabel("Petal Length")
plt.show()
~~~

<img width="543" height="393" alt="image" src="https://github.com/user-attachments/assets/ea3c6acc-7bc8-4f54-99e8-aa228089dc33" />

~~~

# Bar Plot
plt.figure(figsize=(6,4))
df.mean().plot(kind="bar")
plt.title("Average Feature Values")
plt.ylabel("Value")
plt.show()

~~~

<img width="573" height="483" alt="image" src="https://github.com/user-attachments/assets/aeb025dc-3eab-41f0-8c0c-60df37f820e5" />

~~~

# Box Plot
plt.figure(figsize=(6,4))
plt.boxplot(df["sepal width (cm)"])
plt.title("Box Plot")
plt.show()
~~~
<img width="534" height="376" alt="image" src="https://github.com/user-attachments/assets/e7991c59-e4ee-4822-a2b8-30c9b9063b30" />






# Result:
 Include your result here
