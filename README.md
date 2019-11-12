# piopiy_pip
PIP create and publish steps



## Step1 : python3 -m pip install --user --upgrade setuptools wheel

## Step2 : python3 setup.py sdist bdist_wheel

## Step3 : python3 -m pip install --user --upgrade twine

### Test Env
## Step4 : python3 -m twine upload --repository-url https://test.pypi.org/legacy/ dist/*

### Production Env

## Step4 : python3 -m twine upload dist/*




#### Test Install Step
## pip install --index-url https://test.pypi.org/simple/ your-package

### Production Install
## pip install your-package
