
# Assignment-1

## 1. Data Dimensionality
- **Total number of vehicles**: 428
- **Number of attributes**: 12
- **Data Types**:
```
Make            object
Model           object
Type            object
Origin          object
DriveTrain      object
MSRP             int64
EngineSize     float64
Cylinders      float64
Horsepower       int64
MPG_Highway      int64
Weight           int64
Length           int64
```
- **Missing Values**:
```
Make           0
Model          0
Type           0
Origin         0
DriveTrain     0
MSRP           0
EngineSize     0
Cylinders      2
Horsepower     0
MPG_Highway    0
Weight         0
Length         0
```

## 2. Data Visualization

### Scatterplot of MSRP vs Horsepower
The scatterplot below shows the relationship between MSRP and Horsepower.
![Scatterplot](scatterplot.png)

### Bar plot of Number of Vehicles by Make
The bar plot below shows the number of vehicles by each make.
![Barplot](barplot.png)

### Make with the Greatest Number of Vehicles
The make with the greatest number of vehicles is **Toyota**, with a total of **28** vehicles.

## 3. Normalization and Standardization of Horsepower

The table below shows the original, normalized, and standardized values of the Horsepower variable:
```
   Original_Horsepower  Normalized_Horsepower  Standardized_Horsepower
0                  265               0.449649                 0.684503
1                  200               0.297424                -0.221395
2                  200               0.297424                -0.221395
3                  270               0.461358                 0.754187
4                  225               0.355972                 0.127028
```

### Statistical Summary
Here is the statistical summary of the transformed data:
```
       Original_Horsepower  Normalized_Horsepower  Standardized_Horsepower
count           428.000000             428.000000             4.280000e+02
mean            215.885514               0.334626            -7.470660e-17
std              71.836032               0.168234             1.001170e+00
min              73.000000               0.000000            -1.991379e+00
25%             165.000000               0.215457            -7.091854e-01
50%             210.000000               0.320843            -8.202571e-02
75%             255.000000               0.426230             5.451340e-01
max             500.000000               1.000000             3.959670e+00
```

## 4. Discussion

### Differences between Normalization and Standardization
Normalization rescales the data to a range between 0 and 1. It is useful when the goal is to ensure that all features have the same scale, especially in algorithms that are sensitive to the scale of input data. Standardization, on the other hand, transforms the data to have a mean of 0 and a standard deviation of 1, making it appropriate for algorithms that depend on the variance of the data.

### Preferred Transformation Method
In this context, I prefer standardization because it maintains the data distribution while making the features more comparable. This is particularly important for statistical modeling, where the variance and distribution of data play a critical role.
