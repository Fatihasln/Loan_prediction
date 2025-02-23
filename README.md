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

⚠️ Challenges and Solutions
Matplotlib Installation Error:

Resolved version conflicts via pip uninstall matplotlib and pip install --upgrade matplotlib.

Alternative solution: Use virtual environments or version pinning.

Missing Values: No missing values found in the dataset.

📊 Key Findings
Highest correlation with default risk: InterestRate, CreditScore, DTIRatio.

The credit/income feature helped better understand borrower risk profiles.
