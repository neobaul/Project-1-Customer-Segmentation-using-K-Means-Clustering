Step 1: Create and Activate the Virtual Environment

# 1. Create a virtual environment named 'ml_env'
python -m venv ml_env

# 2. Activate the virtual environment
ml_env\Scripts\activate

Step 2: Install the Necessary Packages

pip install numpy pandas scikit-learn matplotlib seaborn notebook

Step 3: Create the requirements.txt File

pip freeze > requirements.txt

or put the following text in the requirements.txt File

numpy
pandas
scikit-learn
matplotlib
seaborn
notebook

Bonus: How to Use Your New Environment in Jupyter

