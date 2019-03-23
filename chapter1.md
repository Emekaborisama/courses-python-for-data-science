---
title: 'Python for Data Science'
description: 'Enjoy your exercise as you grow from zero to hero '
free_preview: true
---

## Example coding exercise

```yaml
type: NormalExercise
key: e8c1edbe67
lang: python
xp: 100
skills: 2
```

# **Hello,Welcome to Day 4- 5 of 100 days of Ds code.** 

We discussed on Python libraries for Data Science and we mentioned 9 of them.([See link here](https://medium.com/100daysofdscode/100daysof-dscode-datascience-day-4-5-python-for-data-science-ab0a04f632a3)).

In this exercise we will focus on the popular and most used data science libraries which are :
1. Pandas
2. Numpy
3. Matplotlib

`@instructions`
Type the 3 most used Python libraries for Data Science

#Check hint if you are having an issue running this exercise

`@hint`
#pandas
#numpy
#matplotlib

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
#pandas
#numpy
#matplotlib
```

`@sct`
```{python}

```

---

## Numpy

```yaml
type: NormalExercise
key: 1f89ed8bc9
xp: 100
```

Wow, **Congrats** ```
:)
``` you have successfully entered the society of ds heros with python as your sword and you got to use your intuition as your skills
In this phase you will write code like a World-class Data Scientist. 
Let's look at the first python library on our list(previous session)

**Numpy**

`@instructions`
Import```Numpy``` library and pass it into an alias
```np``` then use ```np.around```use it to round up the sum of 2.345 + 2.7845 into 2 decimal places.

`@hint`
Import numpy and print (first number+ 2nd number), then use np.around to round them the sum total into 2 decimal places

`@pre_exercise_code`
```{python}
import numpy as np
value = (2.345 + 2.7845)
np.around(value,2)

```

`@sample_code`
```{python}

```

`@solution`
```{python}
import numpy as np
value = (2.345 + 2.7845)
np.around(value,2)
```

`@sct`
```{python}

```

---

## Numpy Exercise

```yaml
type: MultipleChoiceExercise
key: 20ccf0e81e
xp: 50
```

This exercise will requires you to research online 

Research and write 30 Numpy code to perform a task

`@possible_answers`


`@hint`
Click [here](https://www.w3resource.com/python-exercises/numpy/index.php) to see hint

`@pre_exercise_code`
```{python}

```

`@sct`
```{python}

```

---

## Pandas

```yaml
type: NormalExercise
key: 909951eb49
xp: 100
```

Congrats, You have successfully migrate to the second stage of the game to become a world class Data Scientist.

In this Stage we will doing a simple exercise on pandas but before that follow the instruction below

`@instructions`
In this session you will Import```pandas``` library and pass it into an alias
```pd```

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
import pandas as pd
```

`@sct`
```{python}

```

---

## How To Create a Pandas DataFrame

```yaml
type: NormalExercise
key: 20c4d15f4b
xp: 100
```

Apparently, creating dataframe is your first step in almost anything that you want to do when it comes to data munging in Python. Sometimes you will want to start from scratch but you can also convert other data structures, such as lists or Numpy arrays to Pandas DataFrames.

`@instructions`
In this session you will create a pandas dataframe using Numpy arrays ```nparray```.

You are required to just pass it to the ```DataFrame()``` function in the data argument.

Erase the code in the box and retype it(Don't forget practice makes perfect)

`@hint`
nparray

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
#Here is an example of a dataframe made with numpy nparray
import numpy as np
import pandas as pd
data = np.array([['','Col1','Col2'],
                ['Row1',1,2],
                ['Row2',3,4]])
 #Convert a numpy array to Pandas Dataframe               
print(pd.DataFrame(data=data[1:,1:],
                  index=data[1:,0],
                  columns=data[0,1:]))
my_series = pd.Series({"United Kingdom":"London", "India":"New Delhi", "United States":"Washington", "Belgium":"Brussels"})
print(pd.DataFrame(my_series))
.
print("#We have sucessfully created a dataframe in pandas using numpy arrays")
```

`@solution`
```{python}
import numpy as np
import pandas as pd
data = np.array([['','Col1','Col2'],
                ['Row1',1,2],
                ['Row2',3,4]])
 #Convert a numpy array to Pandas Dataframe               
print(pd.DataFrame(data=data[1:,1:],
                  index=data[1:,0],
                  columns=data[0,1:]))
my_series = pd.Series({"United Kingdom":"London", "India":"New Delhi", "United States":"Washington", "Belgium":"Brussels"})
print(pd.DataFrame(my_series))
```

`@sct`
```{python}

```

---

## Pandas Dataframe exercise

```yaml
type: NormalExercise
key: 0269fdf8cd
xp: 100
```

Convert the following numpy arrays to pandas dataframe

`@instructions`
Convert the following to pandas dataframe
```1. my_dict = {1: ['1', '3'], 2: ['1', '2'], 3: ['2', '4']}```
```2.my_series = pd.Series({"United Kingdom":"London", "India":"New Delhi", "United States":"Washington", "Belgium":"Brussels"})```

Check your previous exercise for hint to pass this session.
Don't forget to import libraries first.

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
import numpy as np
import pandas as pd
my_dict = {1: ['1', '3'], 2: ['1', '2'], 3: ['2', '4']}
print(pd.DataFrame(my_dict))
my_series = pd.Series({"United Kingdom":"London", "India":"New Delhi", "United States":"Washington", "Belgium":"Brussels"})
print(pd.DataFrame(my_series))
```

`@sct`
```{python}

```

---

## Know your dataset 1

```yaml
type: NormalExercise
key: d3cb323347
xp: 100
```

Wow, Nice step.
In session we are going to learn a little bit about the data we created

`@instructions`
You will be using ```shape``` and ```len()``` join with index property.

The shape property will provide you with the dimensions of your DataFrame. That means that you will get to know the width and the height of your DataFrame. On the other hand, the len() function, in combination with the index property, will only give you information on the height of your DataFrame.

Erase the code in the box and retype it(Don't forget practice makes perfect)

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
import numpy as np
import pandas as pd

df = pd.DataFrame(np.array([[1, 2, 3], [4, 5, 6]]))

# Use the `shape` property
print(df.shape)

# Or use the `len()` function with the `index` property
print(len(df.index))
```

`@solution`
```{python}
import numpy as np
import pandas as pd
df = pd.DataFrame(np.array([[1, 2, 3], [4, 5, 6]]))
print(df.shape)
print(len(df.index))
```

`@sct`
```{python}

```

---

## Know your dataset 2

```yaml
type: NormalExercise
key: c0163bb980
xp: 100
```

After loading a data you need to see your data. lol imagine your wife just gave birth of course you will need to see your child.

`@instructions`
In this session we will use ```describe``` to generate descriptive statistics that summarize the central tendency, dispersion and shape of a dataset distribution and excluding NaN values.
We can also use
DataFrame.count
Count number of non-NA/null observations.
DataFrame.max
Maximum of the values in the object.
DataFrame.min


Erase the code in the box and retype it(Don't forget practice makes perfect)

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
import pandas as pd 
path='https://ibm.box.com/shared/static/q6iiqb1pd7wo8r3q28jvgsrprzezjqk3.csv'
df = pd.read_csv(path)
df.describe
```

`@solution`
```{python}

```

`@sct`
```{python}

```

---

## How to load data using pandas

```yaml
type: NormalExercise
key: cb79d244dd
xp: 100
```

Yes, You made it through.
In this session we will load a Dataset using Pandas and assign it to a variable

`@instructions`
To load a Dataset you will use  ```pd.read_csv and pd.read_excel('filename.xlsx') e.t.c```.

We will load a Dataset from IBM database using the url and assign a variable to it, then print out the first 5 rows.

Erase the code in the box and retype it(Don't forget practice makes perfect)

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
import pandas as pd 
#url path
path='https://ibm.box.com/shared/static/q6iiqb1pd7wo8r3q28jvgsrprzezjqk3.csv'
#assigning your data to a variable
df = pd.read_csv(path)
#print the first 5  rows
df.head(5)
```

`@solution`
```{python}
import pandas as pd 
path='https://ibm.box.com/shared/static/q6iiqb1pd7wo8r3q28jvgsrprzezjqk3.csv'
df = pd.read_csv(path)
df.head(5)
```

`@sct`
```{python}

```

---

## Tips

```yaml
type: NormalExercise
key: f4e7a396ac
xp: 100
```

```
- DataFrame.isna()	Detect missing values.
DataFrame.notna()	Detect existing (non-missing) values.

DataFrame.head([n])	Return the first n rows.
DataFrame.at	Access a single value for a row/column label pair.
DataFrame.iat	Access a single value for a row/column pair by integer position.
DataFrame.loc	Access a group of rows and columns by label(s) or a boolean array.
DataFrame.iloc	Purely integer-location based indexing for selection by position.
DataFrame.insert(loc, column, value[, …])	Insert column into DataFrame at specified location.

DataFrame.dropna([axis, how, thresh, …])	Remove missing values.
DataFrame.fillna([value, method, axis, …])	Fill NA/NaN values using the specified method.


DataFrame.append(other[, ignore_index, …])	Append rows of other to the end of caller, returning a new object.
DataFrame.assign(**kwargs)	Assign new columns to a DataFrame.
DataFrame.join(other[, on, how, lsuffix, …])	Join columns of another DataFrame.
```

`@instructions`
The code above is useful so write it on your learning notebook and click on submit to pass

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```

---

## Practice

```yaml
type: MultipleChoiceExercise
key: d803aaf772
xp: 50
```

This exercise will requires you to do the following task.

Read the dataset
assign it to a variable ```df```
describe your dataset
count the number of column and rows using the dataset
(Use the IBM dataset given to you)

`@possible_answers`


`@hint`
Read the dataset
assign it to a variable ```df```
describe your dataset
count the number of column and rows using the dataset
(Use the IBM dataset given to you)

`@pre_exercise_code`
```{python}

```

`@sct`
```{python}

```

---

## Matplotlib

```yaml
type: NormalExercise
key: 129e6d4749
xp: 100
```

Wow, Next level ohhhhhh.

In this session you will develop a simple bar chart using matplotlib

`@instructions`
Import matplotlib library and click submit to migrate to the next level

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
import matplotlib.pyplot as plt
```

`@sct`
```{python}

```

---

## Plot

```yaml
type: NormalExercise
key: 41f9f22750
xp: 100
```

Next level ohhhhhh.

In this session you will develop a bar chart using matplotlib but you will do it on your Jupyter notebook or IBM waston notebook(recommended) and submit it here due to the library overfitting on this editor```
(lol:) )
```

`@instructions`
matplotlib.pyplot is a list of command style functions that make matplotlib work like MATLAB. Each pyplot function produces some change to a figure: e.g., creates a figure, creates a plotting area in a figure,plots some lines in a plotting area, decorates the plot with labels, etc.

In this session you will plot a bar chart of the IBM dataset but you will do it on your Jupyter notebook or IBM waston notebook(recommended) and submit it [here](https://goo.gl/forms/Sb0vFEeOyz74tEqf1) due to the library overfitting on this editor```(lol:) )```
.

```Kindly click on submit button to migrate to fly with Qatar Air  :)```

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}
#Here is a tips
import matplotlib.pyplot as plt
plt.plot([1, 2, 3, 4])
plt.ylabel('some numbers')
plt.show()

```

`@solution`
```{python}

```

`@sct`
```{python}

```

---

## Congrats

```yaml
type: NormalExercise
key: 03ce174c7d
xp: 100
```

Welcome to the end of Day 4-5 enthusiast

Wow, we have come to the end of week 1, you are amazing trust me and i am well sure that right now you know:
1. The 10 python libraries for data science, 
2. Have a comprehensible understanding on how to use pandas to read,load and do other activities using pandas,numpy and matplotlib
3. grow in knowledge and intuition

`@instructions`
Kindly type the hashtag you are required to use to share your progress on your social media page.

`@hint`


`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
#100daysofcode #100daysofDscode #100days  #Day2outof100 #DataScience #MachineLearning #Ai
```

`@sct`
```{python}

```
