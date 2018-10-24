# Day 1 Python 

## Aim

To go from gaining new knowledge to comprehension of the foundations of Python and being able to apply this knowledge for data
manipulation and ploting

Programming is a creative process, that uses building blocks
Each instruction you give is a building block, essentially you tell the computer “Do this; then do that.”

## What is Python and Jupyter
https://www.python.org/

https://jupyter.org/

## Folder sctructure
    ├── python-novice
         ├── data   http://swcarpentry.github.io/python-novice-gapminder/files/python-novice-gapminder-data.zip
         └── scripts


    Exercise - New Python notebook script (2 min)

    - Create a new notbook in the `scripts` folder and called it `00_basics` 


## Errors are Okay!
If the computer can't understand the code, it will burp an error message

# Notebooks
    Exercise

    - Create a new notebook called `00_basics` in your `scripts` folder
    - Click on the `Help` option from the top menu and follow the tour `User interface Tour`
    This tour will show you how everything is laid out 
    - What happends when you press `p`?

## Variables

Values can be fixed, calculated or a result of a transformation. Variables follow naming conventions
- s
- h
- n


## Data types
- i
- f
- s
- b


## Methods
help()

`Crtl + c`


## Import files

Let’s introduce some data to Python.
First, make sure you have a data folder!
Remember Python is case sensitive

    Exercise - Reading in files (3 min)

    - Use `pandas.read_csv()`  to import data into Python
    you will store three variables named `africa`, `europe`, `anz` from
    `gapminder_gdp_africa.csv`, `gapminder_gdp_europe.csv`, `gapminder_gdp_oceania.csv` 
    use `index_col='country'`

    - It is recommended that you always use the help to find out more about the new functions before using them

    - Check the function `.info()` with your new variables
    

## DataFrames atributes

No parentesis

- df.columns
- df.axes
- df.dtypes
- df.shape
- df.size
- df.values

## Data Frames methods

- df.info()
- df.describe()
- df.head()
- df.tail()


    Exercise - Americas (2 min)

    - Read the dataset `gapminder_gdp_americas.csv` (which should be in the same directory as `gapminder_gdp_oceania.csv`) and index by `country` into a variable called `americas`
    - After reading the data for the Americas, use `help(americas.head)` and `help(americas.tail)` to find out what `DataFrame.head` and `DataFrame.tail` do.

      - What method call will display the first three rows of this data?
      - What method call will display the last three columns of this data? (Hint: you may need to change your view of the data.)

    - Display its summary statistics of `americas`
   


## Plotting

# Resources

* Python for Biologists: http://www.programmingforbiologists.org/about/why-python/
* Python for psychologists: http://blog.efpsa.org/2016/07/12/python-programming-in-psychology-from-data-collection-to-analysis/
* Biopython: https://biopython.org/
* Python Graph gallery: https://python-graph-gallery.com/matplotlib/
* https://www.amazon.com/Python-Biologists-complete-programming-beginners/dp/1492346136
* https://www.amazon.com/Python-Data-Analysis-Wrangling-IPython/dp/1491957662]
* Jupyter install https://jupyter.org/install
* Jupyter 2 or 3 https://stackoverflow.com/questions/28831854/how-do-i-add-python3-kernel-to-jupyter-ipython
* python 3.7 https://stackoverflow.com/questions/51279791/how-to-upgrade-python-version-to-3-7
* python 3.7 https://superuser.com/questions/241865/updating-python-on-ubuntu-system
* Reproducibility mybinder https://mybinder.org/
* Reproducibility codeocean https://codeocean.com/
* Mybinder example https://hub.mybinder.org/user/binder-examples-nda_environment-6kif41cf/notebooks/index.ipynb
* Python DataFrame https://pandas.pydata.org/pandas-docs/stable/generated/pandas.DataFrame.html
* Pandas cheatsheet https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf
* Pandas cheatsheet dataquest https://www.dataquest.io/blog/large_files/pandas-cheat-sheet.pdf
* Pandas cheatsheet datacamp https://s3.amazonaws.com/assets.datacamp.com/blog_assets/PandasPythonForDataScience+(1).pdf
* Python matplotlib https://matplotlib.org/users/dflt_style_changes.html
* Python Style guide https://www.python.org/dev/peps/pep-0008/
