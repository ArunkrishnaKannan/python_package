
# Build you own Python Library

In this Library file we have created the first library module as simple arithmetic operations like Addition, Subtraction, Multiplication, Division as basic 2 sum of calculator

## Step 1: Download Python and VS Code

1. Get into the Python official website and download the latest version of python  
https://www.python.org/

2. Next get into the Visual Studio code official website and download the latest version based on your OS
https://code.visualstudio.com/download
## Step 2: Open the Visual Studio Code and Create folder

1. Create the folder like "Basic_Calculator" inside that create a folder like "yourname-calculator" and inside create file __init__.py 

2. Add a piece of code like def a function with 2 numbers and return the addition, Subtraction, Multiplication, Division



## Step 3: Create a Supporting files

1. Create a file Called CHANGELOG.txt and add the versions of the package and release date

2. Create the LICENSE.txt file in here we should add the MIT opensource license click the below link and copy the copyright part and paste it in LICENSE.txt
https://opensource.org/license/mit-0

3. Create the MANIFEST.in file in there we should include globally a txt and python files to build the package

4. Create a README.txt file it will be just show the description of the package.

5. Create a setup.py file in there is file we should add our project name, version, description, author and license details it only makes the package to run the python file init.py after build process.

## Create a account in pypi

1. Go to https://pypi.org/account/register/ add your details and create an account 
2. Make sure to enable 2FA authentication if it is not enabled the API token will not be created and we cannot upload our packages

## Go to Powershell 

1. Open the Powershell and install the twine

twine - Twine is a command-line tool used to securely upload Python packages to PyPI (Python Package Index) or any private Python package repository.

Command Line -- pip install twine


2. Install the setuptools 

Command Line - pip3 install setuptools twine

👉 Install the tools needed to build (setuptools) and upload (twine) a Python package to PyPI.

3. Next step get into the directory where the basic_calculator python folder is there 

Command Line - Cd ./your-directory/

4. Build the sdist folder of setup file

Command Line - python setup.py sdist

sdist - Stands for Source Distribution.

It tells Python to "build a source package" of your project.

5. Upload the file into pypi as package

Command Line - twine upload --repository-url https://upload.pypi.org/legacy/ dist/*

It will ask API token add the token which you download while creating pypi account and 2FA verification once you give the API token the file will be upload to as package.
