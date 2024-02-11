## Dependencies

1. Clone Repository: https://github.com/duffydata/corporate-action-helper.git 

2. Set up Virtual Enviroment using the following command:  

python3 -m venv venv
 
source venv/bin/activate

3. We use poetry for managing dependencies. To install Poetry please follow the below steps: 

poetry env use python3.x  # use versions greater than 3.8
poetry install
poetry shell
poetry add ipywidgets
jupyter nbextension enable --py widgetsnbextension --sys-prefix
jupyter nbextension enable --py widgetsnbextension --sys-prefix
jupyter nbextension enable --py widgetsnbextension --sys-prefix
jupyter nbextension enable --py widgetsnbextension --sys-prefix
poetry add voila


# Run Voila for a specific notebook

Voila is a great extension to 'productionise jupyter notebooks'. Used with  Ipywidgets, your notebooks turn into interactive dashboards. 
To use Voila follow below steps: 

poetry run voila CorporateActionCalculator.ipynb
 
A local version of the notebook should be now automatically generated using Voila 

# Corporate Action Calculator

Theoretical Open Price Calculator (TOPC) serves as a valuable tool for efficiently computing the Theoretical Open Price of securities on the ex-date of a Corporate Action. This notebook provides a quick efficient way of calculating theoretical open prices for various Corporate Actions, including Cash Dividends, Splits, Rights Issues, and Spin Offs.

Designed for utilization by execution desks, middle offices, back offices, and data analysts engaged in the management of Equities Corporate Action data, this notebook can evaluate the accuracy and completeness of corporate action data. It proves particularly useful for identifying potential gaps or inaccuracies in the provided information.

Please note the functionality of this notebook is centered around the calculation of theoretical open prices and does not intend to determining the actual open price of a security. Factors influencing the actual open price, such as supply and demand dynamics, sentiment, and economic data, fall outside the scope of this tool.

## How To Use

Simply find the type of Corporate Action and populate the fields to generate the theoretical open price

Number 1 for Cash Dividends, Special Cash Dividends, Return of Capital

Number 2 for Splits, Reverse Splits, and Cash Dividend and Split. 

Number 3 for Rights Issues

Number 4 Spin Offs

