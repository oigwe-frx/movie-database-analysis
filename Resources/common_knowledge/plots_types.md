# Types of Plots

## Pandas Plots:

### Line Plot

Method: DataFrame.plot()
Best Used For: Univariate (single variable) or multivariate (multiple variables) data to visualize trends and changes over time.

Parameters:
x (optional): x-axis data (usually a column name or index).
y (optional): y-axis data (usually a column name or index).

Example:
```
  import pandas as pd
  import matplotlib.pyplot as plt
  
  data = {'x': [1, 2, 3, 4, 5], 'y': [10, 14, 8, 18, 12]}
  df = pd.DataFrame(data)
  df.plot(x='x', y='y', kind='line')
  plt.show()
```

### Bar Plot

Method: DataFrame.plot(kind='bar')
Best Used For: Univariate data for comparing discrete categories or displaying frequency counts.

Parameters:
x (optional): x-axis data (usually a categorical column).
y (optional): y-axis data (usually a numerical column).

```
  import pandas as pd
  import matplotlib.pyplot as plt
  
  data = {'Category': ['A', 'B', 'C', 'D'], 'Values': [10, 14, 8, 18]}
  df = pd.DataFrame(data)
  df.plot(x='Category', y='Values', kind='bar')
  plt.show()
```

### Histogram

Method: DataFrame.plot(kind='hist')
Best Used For: Univariate data to display the distribution of a single continuous variable.

Parameters:
- x (optional): x-axis data (usually a numerical column).
- bins (optional): Number of bins for the histogram.

```
  import pandas as pd
  import matplotlib.pyplot as plt

  data = {'Values': [10, 14, 8, 18, 12, 16, 20, 22, 24, 28]}
  df = pd.DataFrame(data)
  df.plot(y='Values', kind='hist', bins=5)
  plt.show()
```

### Box Plot

Method: DataFrame.plot(kind='box')
Best Used For: Univariate or multivariate data to identify outliers and visualize the spread of data.

### Scatter Plot

Method: DataFrame.plot(kind='scatter')
Best Used For: Bivariate (two variables) data to investigate the relationship between two continuous variables.

### Pie Chart

Method: DataFrame.plot(kind='pie')
Best Used For: Univariate data to show the composition of a whole as parts.

### Area Plot

Method: DataFrame.plot(kind='area')
Best Used For: Multivariate data to display cumulative values of multiple variables over time.


## MATLAB Plots:

### Line Plot

Function: plot()
Best Used For: Univariate or multivariate data to visualize trends and data over time.

### Bar Plot

Function: bar()
Best Used For: Univariate data for comparing discrete categories or displaying frequency counts.

### Histogram

Function: hist()
Best Used For: Univariate data to visualize the distribution of a single continuous variable.

### Box Plot

Function: boxplot()
Best Used For: Univariate or multivariate data to identify outliers and visualize the spread of data.

### Scatter Plot

Function: scatter()
Best Used For: Bivariate data to investigate the relationship between two continuous variables.

### Pie Chart

Function: pie()
Best Used For: Univariate data to show the composition of a whole as parts.

### Area Plot

Function: area()
Best Used For: Multivariate data to display cumulative values of multiple variables over time.

### Heatmap

Function: heatmap()
Best Used For: Multivariate data to visualize relationships between two continuous variables using color intensity.

### Contour Plot

Function: contour()
Best Used For: Multivariate data to visualize 3D data on a 2D plane using contour lines.

### Surface Plot

Function: surf()
Best Used For: Multivariate data to visualize 3D data as a surface.
