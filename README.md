# General Information
This is my second university project in which I develop software required to conduct a mathematical research on smoothing data noises using modified least squares method.<br /><br />
To launch the application run the "interface.py" file.

# About the application
The application is developed for researching different aspects of noise smoothing using least squares method modified to use a window with changing length instead of the entire dataset. All the code was written in Python 3.10.4 uisng such modules as<br /><br /> - tkinter<br /> - sympy<br /> - matplotlib<br /> - math<br /> - pandas<br /> - numpy <br /><br />
# Smoothing with fixed window length
![LocalLS_SpeedX2](https://github.com/x-wheel-of-fortune/Least_squares_smoothing_science_research_2022-2023/assets/35616551/570be6a7-549a-42b3-acd5-e5d1db9d7838)
# Smoothing with dynamic window length
![Новый_проект_AdobeExpress](https://github.com/x-wheel-of-fortune/Least_squares_smoothing_science_research_2022-2023/assets/35616551/718c3034-fc8d-4302-9244-e209cf9ab2cd)



### The application consists of two main blocks: generator and approximator.
# Generator
The generator allows you to create sets of points in two-dimensional space based on elementary mathematical functions. The points are saved to a Microsoft Excel table. The generator has a large number of customizable parameters, including the function on the basis of which the points are generated, the interval on which the points will lie, the number of points. The distribution of points on the interval can be regulated - they can be distributed evenly or with a random step. In addition, there is a possibility to generate intervals filled only partially, the percentage of their filling can change dynamically within the specified limits. Noise is applied to the resulting set after generation. It may be a percentage of the original value or an absolute value, may have a uniform or normal distribution with specified parameters. Outliers with adjustable frequency and values can also be added.
<br /><br />
![image](https://user-images.githubusercontent.com/35616551/236660425-429e42ee-faca-4527-84cf-8998a0ee4dfb.png)
<br /><br />
# Approximator
In the approximator block several regression algorythms were programmatically implemented allowing to set various approximation parameters, such as selection of approximation leverage - fixed or dynamic, manual setting of leverage, ability to find an optimal fixed leverage using sequential search of all values, dichotomy or golden section method (which parameters are set manually to avoid stucking in the local minimum). The possibility of data smoothing by dynamic leverage with selection of the optimal vector of shoulders using all variants, random sampling, dichotomy, the Golden Ratio method, as well as a genetic algorithm is implemented. There is an opportunity to stop the process of selecting the optimum leverage, without waiting for its completion to get the best calculated by the moment result. In addition, for the dynamic and fixed arm there is an opportunity to smooth the ends of the graph by moving the point of depreciation from the center to the edge. The possibility to select different methods of calculation of the deviation such as the sum of squares, the sum of modules and the standard deviation is implemented; there is an opportunity not to take the chart ends into account when calculating the deviation. Visualization options of the approximation process allow you to connect the smoothed points with a line, show the actual function by which the points with noise were generated, automatically save the graph with the approximation result on the selected path. It is possible to approximate data by alternative algorithms within one figure. It is possible to show the animation of the approximation process in real time.
<br /><br />
![image](https://user-images.githubusercontent.com/35616551/236660504-3ed13c88-c2d2-403d-8954-97b0b895569c.png)
<br /><br />
