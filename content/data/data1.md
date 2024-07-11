---
title: "List of Irregular Verbs Across Romance Languages" 
date: 2013-03-07
lastmod: 2024-05-08
tags: ["Romance languages","philology","irregular verbs","Portuguese","Italian","French","Spanish","dataset","python"]
author: ["Patrick Fitzcarron O'Leary","Florianus Prinzel","Walter Schoeffler-Henschell","Detlev Amadeus Unterholzer", "Dieter Vogelsang","Moritz-Maria von Igelfeld"]
description: "This dataset contains all irregular verbs in known Romance languages."
summary: "This dataset contains all irregular verbs in known Romance languages."
editPost:
    URL: "https://github.com/pmichaillat/hugo-website"
    Text: "GitHub repository"
showToc: true
disableAnchoredHeadings: false

---

## Overview

This dataset contains all irregular verbs in [all known Romance languages](http://www.alexandermccallsmith.com/series/von-igelfeld-series)—including Portugese, Spanish, French, and Italian. Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

---

## View datasets

+ [Irregular verbs in Portugese](https://github.com/pmichaillat/u-star)
+ [Irregular verbs in Italian](https://github.com/pmichaillat/unemployment-gap)
+ [Irregular verbs in French](https://github.com/pmichaillat/job-rationing)
+ [Irregular verbs in Spanish](https://github.com/pmichaillat/countercyclical-multiplier)

---

## Source of data

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

---

## Description of variables

|  Symbol  |   Range   |  Variable |                        Note                        |
| -------- | --------- | --------- | -------------------------------------------------- |
| $\alpha$ | 1930–1954 | Tempor    | Lorem ipsum dolor sit amet                         |
| $\beta$  | 1930–1954 | Fugiat    | Consectetur adipisicing elit                       |
| $\gamma$ | 1833–1954 | Duis      | Sed do eiusmod                                     |
| $\zeta$  | 1930–1994 | Excepteur | Tempor incididunt ut labore et dolore magna aliqua |
| $\nu$    | 1990–2023 | Lorem     | Ut enim ad minim veniam                            |
| $\chi$   | 1990–2023 | Labore    | Quis laboris nisi ut aliquip ex ea commodo         |
| $\Omega$ | 1890–1900 | Pariatur  | Excepteur sint $\beta > \alpha$                    |

---

## Using data with Python

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

### Start Python:

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua.

```python
import numpy as np
import pandas as pd
```

### Open the file:

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

```python
file_path = 'data.csv'
with open(file_path, 'r') as file:
```

### Read data:

Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur.

```python
    lines = file.readlines()
```

### Parse and process data:

Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur.

```python
data = []
for line in lines:
    line_data = line.strip().split(',')  # Split the line into a list of values
    line_data = [float(value) for value in line_data]  # Convert values to floats
    data.extend(line_data)  # Extend the main list with values from the line
```

#### Compute summary statistics using NumPy:

Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

```python
data_array = np.array(data)  # Convert the list to a NumPy array
mean = np.mean(data_array)
median = np.median(data_array)
std_dev = np.std(data_array)
min_value = np.min(data_array)
max_value = np.max(data_array)
```

#### Display summary statistics:

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat.

```python
print(f"Mean: {mean}")
print(f"Median: {median}")
print(f"Standard Deviation: {std_dev}")
print(f"Minimum Value: {min_value}")
print(f"Maximum Value: {max_value}")
```

### Additional references on unrelated topics

| Title | Author | Year | Link |
| :----- | :------: | :----: | :----: |
| Do Matching Frictions Explain Unemployment? Not in Bad Times | P. Michaillat | 2012 | [pascalmichaillat.org/1.pdf](https://pascalmichaillat.org/1.pdf) | 
| A Theory of Countercyclical Government Multiplier | P. Michaillat | 2014 | [pascalmichaillat.org/2.pdf](https://pascalmichaillat.org/2.pdf) | 
| A Macroeconomic Approach to Optimal Unemployment Insurance: Theory| C. Landais et al.  | 2018 | [pascalmichaillat.org/4.pdf](https://pascalmichaillat.org/4.pdf) | 
| A Macroeconomic Approach to Optimal Unemployment Insurance: Applications | C. Landais et al.  | 2018 | [pascalmichaillat.org/5.pdf](https://pascalmichaillat.org/5.pdf) | 
| Persistence of False Paradigms in Low-Power Sciences | G. Akerlof & P. Michaillat | 2018 | [pascalmichaillat.org/10.pdf](https://pascalmichaillat.org/10.pdf) | 
| Resolving New Keynesian Anomalies with Wealth in the Utility Function | P. Michaillat & E. Saez | 2021 | [pascalmichaillat.org/11.pdf](https://pascalmichaillat.org/11.pdf) | 
| Modeling Job Stealing | P. Michaillat | 2023 | [pascalmichaillat.org/14.pdf](https://pascalmichaillat.org/14.pdf) | 