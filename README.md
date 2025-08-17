 Analysis Steps
Data Loading and Initial Exploration:

Dataset read using pandas.

Data structure inspected with df.head(), df.shape, df.info(), and df.describe().

Missing values checked (df.isnull().sum()).

Target Variable Analysis:

Distribution of the Default column analyzed (11.6% default rate).

Numerical Variable Analysis:

Numerical columns isolated (df_numeric = df.select_dtypes(include=["int64", "float64"])).

Correlation matrix and heatmap generated using matplotlib/seaborn.

Feature Engineering:

New feature created: credit/income (Loan Amount / Income).

credit/income variable categorized into four groups: Low, Medium, High, Very High.

Visualization:

Distribution plots and categorical analyses performed.


