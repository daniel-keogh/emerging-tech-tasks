# Emerging Technologies Tasks

Y4S1 Emerging Technologies Tasks Assessment

## Running

You can run the notebook by first installing [Anaconda](https://www.anaconda.com/) and then executing the below command from within the repository's root directory.

```sh
$ jupyter notebook
```

## Tasks

### 1. Square Root of 2

Write a Python function called `sqrt2` that calculates and prints to the screen the square root of 2 to 100 decimal places. Your code should not depend on any module from the standard library or otherwise. You should research the task first and include references and a description of your algorithm.

### 2. Chi-squared Test for Independence

The Chi-squared test for independence is a statistical hypothesis test like a *t*-test. It is used to analyse whether two categorical variables are independent. The [Wikipedia](https://en.wikipedia.org/w/index.php?title=Chi-squared_test&oldid=983024096) article gives the table below as an example, stating the Chi-squared value based on it is approximately 24.6. Use `scipy.stats` to verify this value and calculate the associated *p* value. You should include a short note with references justifying your analysis in a markdown cell.

|   | A | B | C | D | Total |
| - | - | - | - | - | ----- |
| White collar | 90 | 60 | 104 | 95 | 349 |
| Blue collar  | 30 | 50 | 51 | 20 | 151 |
| No collar    | 30 | 40 | 45 | 35 | 150 |
| **Total**        | 150 | 150 | 200 | 150 | 650 |

### 3. Standard Deviation

The standard deviation of an array of numbers `x` is calculated using `numpy` as `np.sqrt(np.sum((x - np.mean(x))**2)/len(x))`. However, Microsoft Excel has two different versions of the standard deviation calculation, `STDEV.P` and `STDEV.S`. The `STDEV.P` function performs the above calculation but in the `STDEV.S` calculation the division is by `len(x)-1` rather than `len(x)`. Research these Excel functions, writing a note in a Markdown cell about the difference between them. Then use `numpy` to perform a simulation demonstrating that the `STDEV.S` calculation is a better estimate for the standard deviation of a population when performed on a sample. Note that part of this task is to figure out the terminology in the previous sentence.

### 4. k-means Clustering with the Iris Dataset

Use `scikit-learn` to apply k-means clustering to Fisher's famous Iris data set. You will easily obtain a copy of the data set on-line. Explain in a Markdown cell how your code works and how accurate it might be, and then explain how your model could be used to make predictions of species of iris.
