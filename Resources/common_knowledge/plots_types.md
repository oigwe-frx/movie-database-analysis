# Types of Plots

## Pandas Plots:

Sure, here's the list of various types of pandas and MATLAB plots in markdown format with details, parameters, and examples:

## Pandas Plots

### Line Plot

- Method: `DataFrame.plot()`
- Best Used For: Univariate (single variable) or multivariate (multiple variables) data to visualize trends and changes over time.
- Parameters:
  - `x` (optional): x-axis data (usually a column name or index).
  - `y` (optional): y-axis data (usually a column name or index).

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'x': [1, 2, 3, 4, 5], 'y': [10, 14, 8, 18, 12]}
df = pd.DataFrame(data)
df.plot(x='x', y='y', kind='line')
plt.show()
```

### Bar Plot

- Method: `DataFrame.plot(kind='bar')`
- Best Used For: Univariate data for comparing discrete categories or displaying frequency counts.
- Parameters:
  - `x` (optional): x-axis data (usually a categorical column).
  - `y` (optional): y-axis data (usually a numerical column).

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'Category': ['A', 'B', 'C', 'D'], 'Values': [10, 14, 8, 18]}
df = pd.DataFrame(data)
df.plot(x='Category', y='Values', kind='bar')
plt.show()
```

### Histogram

- Method: `DataFrame.plot(kind='hist')`
- Best Used For: Univariate data to display the distribution of a single continuous variable.
- Parameters:
  - `x` (optional): x-axis data (usually a numerical column).
  - `bins` (optional): Number of bins for the histogram.

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'Values': [10, 14, 8, 18, 12, 16, 20, 22, 24, 28]}
df = pd.DataFrame(data)
df.plot(y='Values', kind='hist', bins=5)
plt.show()
```

### Box Plot

- Method: `DataFrame.plot(kind='box')`
- Best Used For: Univariate or multivariate data to identify outliers and visualize the spread of data.
- Parameters:
  - `by` (optional): Group data by a specific column.

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'Category': ['A', 'A', 'B', 'B', 'C', 'C'], 'Values': [10, 14, 8, 18, 12, 16]}
df = pd.DataFrame(data)
df.plot(x='Category', y='Values', kind='box')
plt.show()
```

### Scatter Plot

- Method: `DataFrame.plot(kind='scatter')`
- Best Used For: Bivariate (two variables) data to investigate the relationship between two continuous variables.
- Parameters:
  - `x` (optional): x-axis data (usually a numerical column).
  - `y` (optional): y-axis data (usually a numerical column).

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'X': [1, 2, 3, 4, 5], 'Y': [10, 14, 8, 18, 12]}
df = pd.DataFrame(data)
df.plot(x='X', y='Y', kind='scatter')
plt.show()
```

### Pie Chart

- Method: `DataFrame.plot(kind='pie')`
- Best Used For: Univariate data to show the composition of a whole as parts.
- Parameters:
  - `y` (optional): Data to plot as pie slices (usually a numerical column).

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'Category': ['A', 'B', 'C'], 'Values': [30, 45, 25]}
df = pd.DataFrame(data)
df.plot(y='Values', kind='pie', labels=df['Category'], autopct='%1.1f%%')
plt.show()
```

### Area Plot

- Method: `DataFrame.plot(kind='area')`
- Best Used For: Multivariate data to display cumulative values of multiple variables over time.
- Parameters:
  - `x` (optional): x-axis data (usually a column name or index).
  - `y` (optional): y-axis data (usually one or more columns).

```python
import pandas as pd
import matplotlib.pyplot as plt

data = {'x': [1, 2, 3, 4, 5], 'A': [10, 14, 8, 18, 12], 'B': [5, 9, 7, 15, 10]}
df = pd.DataFrame(data)
df.plot(x='x', y=['A', 'B'], kind='area')
plt.show()
```

Certainly! Here's the list of various types of MATLAB plots in markdown format with details, parameters, and examples:

## MATLAB Plots

### Line Plot

- Function: `plot()`
- Best Used For: Univariate or multivariate data to visualize trends and data over time.
- Parameters:
  - `x` (optional): x-axis data.
  - `y` (optional): y-axis data.

```matlab
x = [1, 2, 3, 4, 5];
y = [10, 14, 8, 18, 12];
plot(x, y)
xlabel('X-axis')
ylabel('Y-axis')
title('Line Plot Example')
grid on
```

### Bar Plot

- Function: `bar()`
- Best Used For: Univariate data for comparing discrete categories or displaying frequency counts.
- Parameters:
  - `x` (optional): x-axis data.
  - `height` (optional): Heights of the bars.

```matlab
categories = {'A', 'B', 'C', 'D'};
values = [10, 14, 8, 18];
bar(categories, values)
xlabel('Categories')
ylabel('Values')
title('Bar Plot Example')
grid on
```

### Histogram

- Function: `hist()`
- Best Used For: Univariate data to visualize the distribution of a single continuous variable.
- Parameters:
  - `x` (optional): Data to be plotted as a histogram.
  - `nbins` (optional): Number of bins for the histogram.

```matlab
data = [10, 14, 8, 18, 12, 16, 20, 22, 24, 28];
hist(data, 5)
xlabel('Values')
ylabel('Frequency')
title('Histogram Example')
grid on
```

### Box Plot

- Function: `boxplot()`
- Best Used For: Univariate or multivariate data to identify outliers and visualize the spread of data.
- Parameters:
  - `x` (optional): Data to be plotted as a box plot.

```matlab
data = [10, 14, 8, 18, 12, 16, 20, 22, 24, 28];
boxplot(data)
xlabel('Data')
ylabel('Values')
title('Box Plot Example')
grid on
```

### Scatter Plot

- Function: `scatter()`
- Best Used For: Bivariate data to investigate the relationship between two continuous variables.
- Parameters:
  - `x` (optional): x-axis data.
  - `y` (optional): y-axis data.

```matlab
x = [1, 2, 3, 4, 5];
y = [10, 14, 8, 18, 12];
scatter(x, y)
xlabel('X-axis')
ylabel('Y-axis')
title('Scatter Plot Example')
grid on
```

### Pie Chart

- Function: `pie()`
- Best Used For: Univariate data to show the composition of a whole as parts.
- Parameters:
  - `X` (optional): Data to be plotted as pie slices.

```matlab
categories = {'A', 'B', 'C'};
values = [30, 45, 25];
pie(values, categories)
title('Pie Chart Example')
```

### Area Plot

- Function: `area()`
- Best Used For: Multivariate data to display cumulative values of multiple variables over time.
- Parameters:
  - `x` (optional): x-axis data.
  - `y` (optional): y-axis data.

```matlab
x = [1, 2, 3, 4, 5];
A = [10, 14, 8, 18, 12];
B = [5, 9, 7, 15, 10];
area(x, [A', B'])
xlabel('X-axis')
ylabel('Y-axis')
title('Area Plot Example')
grid on
```

These examples should help you understand how to use various MATLAB plot types with their respective parameters in markdown format.
