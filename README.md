# Alpha Research and Factor Modeling

### Project Motivation:

1. To build a statistical risk model using Principal Component Analysis (PCA).
2. To construct a portfolio of equities using the PCA model along with 5 alpha factors.
3. The factors are evaluated using factor-weight returns, quantile analysis, Sharpe Ratio, and turnover analysis.
4. To optimize the portfolio using the risk model and factors.

### The notebook is separated into three parts:
1. The first part covers data collection and inspection, stock universe construction, fitting a PCA model, creating a statistical risk model based on calculating factor returns, covariance matrix, and idosyncratic variance matrix from the PCA model, and finally predicting portfolio risk based on the risk model.
    - note this project makes specific use of the Zipline library which was created by Quantopian, a crowd-sourced investment fund, which closed in 2020. The library is still maintained by Stefan Jansen, author of the book 'Machine Learning for Algorithmic Trading.' See [zipline homepage](https://zipline.ml4trading.io/) for specifics.
2. The second part covers research and creation of five different alpha factors, evaluating each factor's performance, and turnover analysis.
3. The third part covers construction of an optimal equities portfolio that trades as close as possible to the alphas researched and created in part two, but limiting risk as measured by the risk model formed in part one.

### File Descriptions:


    project_4.ipynb
    | - Jupyter notebook containing all data collection, cleaning, and data frame construction, PCA and risk model construction, alpha factor research, construction, and performance evaluation, and finally creating and evaluating an optimal portfolio to minimize risk and trade as close to the alphas as possible.
    helper.py
    |- helper file to abstract some data collection and import statements
    project_helper.py
    |- helper file to abstract graphing functions
    project_test.py
    |- unit tests to flag any major errors
    README.md


### Installations:
- This project uses the 'Zipline' library to generate the dataset used in this project. Zipline was created by Quantopian, a crowd-sourced investment fund, which closed in 2020. The library is still maintained by Stefan Jansen, author of the book 'Machine Learning for Algorithmic Trading.' See [zipline homepage](https://zipline.ml4trading.io/) for specifics.
- You will need a python environment with the following:
    - see the `requirements.txt` file for specific packages and versions
    - python verson 3.7 or higher

### Instructions:
1. Run each cell in 'project_4.ipynb' in sequence. Make sure the Jupyter notebook is in the same level of the directory as 'helper.py', 'project_helper.py', 'project_tests.py', and 'tests.py'.
