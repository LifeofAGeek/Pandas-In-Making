# Pandas-In-Making
Building a Data Analysis Library similar to Pandas from Scratch.

This repository contains a detailed project, how to build our own Python data analysis library from scratch. The end result will be a fully-functioning library very similar to pandas.

## Pre-Requisites

* Basic types and common data structures (lists, tuples, sets, and dictionaries)
* Control flow with if/else statements and for loops (especially when iterating through lists or dictionaries)
* Raising and handling exceptions
* Basics of classes and object-oriented programming.
* Numpy library.

## Objectives

* Have a DataFrame class with data stored in numpy arrays
* Select subsets of data with the brackets operator
* Use special methods defined in the Python data model
* Have a nicely formatted display of the DataFrame in the notebook
* Implement aggregation methods - sum, min, max, mean, median, etc...
* Implement non-aggregation methods such as isna, unique, rename, drop
* Group by one or two columns
* Have methods specific to string columns
* Read in data from a comma-separated value file

### Command to create new environment

In the top level directory of this repository, where the `environment.yml` file is located, run the following from your command line.

`conda env create -f environment.yml`

The above command will take some time to complete. Once it completes, the environment will be created.

### List the environments

Run the command `conda env list` to show all the environments you have. There will be a `*` next to the active environment, which will likely be `base`, the default environment that everyone starts in.

### Activate the pandas_cub environment

Creating the environment does not mean it is active. You must activate in order to use it. Use the following command to activate it.

`conda activate pandas_cub`

You should see `pandas_cub` in parentheses preceding your command prompt. You can run the command `conda env list` to confirm that the `*` has moved to `pandas_cub`.

### Deactivate environment

You should only use the `pandas_cub` environment to develop this library. When you are done with this session, run the command `conda deactivate` to return to your default conda environment.

## Test-Driven Development with pytest

The completion of each part of this project is predicated upon passing the
tests written in the `test_dataframe.py` module inside the `tests` folder.

We will rely upon the [pytest library][1] to test our code. We installed it along with a command line tool with the same name during our environment creation.

[Test-Driven development][3] is a popular approach for developing software. It involves writing tests first and then writing code that passes the tests.

### Testing

All the tests have already been written and are located in the `test_dataframe.py` module found in the `tests` directory. There are about 100 tests that you will need to pass to complete the project. To run all the tests in this file run the following on the command line.

`$ pytest tests/test_dataframe.py`

If you run this command right now, all the tests will fail. You should see a line of red capital 'F's. As you complete the steps in the project, you will start passing the tests. There are about 100 total tests. Once all the tests are passed, the project will be complete.

