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

We discussed on Python libraries for Data Science and we mentioned 10 of them.
in this exercise we will focus on the popular and most used data science libraries such as 
1. Pandas
2. Numpy
3. Matplotlib
4. Scapy

`@instructions`
Type the 4 most used Python libraries for Data Science

`@hint`
PNMS

`@pre_exercise_code`
```{python}

```

`@sample_code`
```{python}

```

`@solution`
```{python}
Pandas
Numpy
Matplotlib
Scapy
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

Apparently, creating dataframe is your first step in almost anything that you want to do when it comes to data munging in Python. Sometimes, you will want to start from scratch, but you can also convert other data structures, such as lists or Numpy arrays, to Pandas DataFrames. 

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
data = np.array([['','Col1','Col2'],
                ['Row1',1,2],
                ['Row2',3,4]])
 #Convert a numpy array to Pandas Dataframe               
print(pd.DataFrame(data=data[1:,1:],
                  index=data[1:,0],
                  columns=data[0,1:]))
```

`@solution`
```{python}

```

`@sct`
```{python}

```
