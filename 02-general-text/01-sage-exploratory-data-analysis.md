# Exploratory Data Analysis

* **Exploratory Data Analysis**
    * John W. Tukey
    * **Data Analysis Strategies**
        * Graphical Representation
        * Flexibility in viewpoints
        * Search for parsimony and simplicity
    * In EDA flexibility is important to adapt what is calculated to the needs of the situation and the clues that were already provided by the data analysis
    * "Histogram is old-fashioned"
    * EDA doesn't need probability, significance or confidence
    * EDA is actively incisive rather than passively descriptive. Emphasis on discovery of unexpected
    * EDA is a willingness to look for things that we believe are not there, as well as those we believe to be there
    * EDA isolates patterns and features of the data
    * Short definition of EDA
        * Attitude
        * Flexibility
        * Graph paper
    * In EDA we search for displays and quantities that provide insights, understanding and surprises
<br><br>
* **Table**
    * Simples EDA object
    * Arranges data in a convenient form
* **Five-Number Summary**
    * In Portuguese, "Resumo dos Cinco Números"
    * From a batch of numbers, those five number summarize the data
        * Minimum
        * Lower Quartile
        * Median
        * Upper Quartile
        * Maximum
    * Auditing a dataset
    * Getting a feel from data
* **Stem-and-Leaf Display**
    * In Portuguese, "Diagrama de Ramos e Folhas"
    * Condensantion of datasets
* **Scatterplot Matrix**
    * In Portuguese, "Gráfico de Dispersão"
* **Outlier**
    * An observation too far from the central value
    * Unnusual value relative to the bulk of data
    * Those values affect directly averages and least squares lines
    * **Boxplot**
        * In Portuguese, "Diagrama de Caixa"
        * Rectangle with top and bottom at the level of quartiles
        * Horizontal line at the level of median
        * Whiskers at top and bottom, 1.5 times the interquartile range
        * Points outside those limits are potential outliers
        * *Parallel box plots*
            * More than one box plot in a figure
* **Residual Plot**
    * Residuals are the difference between data and their corresponding fitted values in a line fit through data
    * Potential outliers are the points with most residuals
* **Bag Plot**
    * Bivariate data
    * Generalization of box plot
    * Studies the scatter of bivariate data
    * Construction of a bag plot
        * Bivariate median
        * Analog of quartiles
        * Whiskers
    * Center of Bag Plot
        * Tukey median
    * The "bag" surrounds the center, containing 50% of observations with greatest depth
    * The "fence" separates inliers from outliers
    * Whiskers are lines marking observations between bag and fence
    * The fence is obtained inflating the bag from the center, by a factor 3
    * Bag plot is resistant to outliers
        * Unusual points doesn't affect the bag plot location or shape
* **Smoother**
    * Replaces a scatter of points by a smooth curve
    * Local character is introduced by employing a kernel
    * A second kernel makes the operation robust or resistant
        * Reduces the impact of points with large residuals
    * **Robust Variant**
        * Robust smooth
            * Obtain a curve not strongly affected by outliers
        * Loess procedure
            * Robust/resistant variant
* **Reexpression**
    * Expressing same information by different numbers
    * Example of using a logarithm scale
    * Purposes
        * Additivity
        * Obtaining straightness or symmetry
        * Making variability more uniform
* **Median Polish**
    * Two-way tables
    * Process of llternately finding and subtracting medians from rows and columns until the results do not change much
    * Purpose of seeking an additive model for two-way table, in the presence of outliers
<br><br>
* **Data Visualization**
    * Objective of providing efficient graphical display for summarizing and reasoning about quantitative information
* **Object-Feature table**
    * Rows represent an observation of object
    * Columns correspond to numerical feature or indicator for the whole set