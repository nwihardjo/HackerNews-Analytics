Below are setup instructions for the Big Data course. The prefered OS is Unix based (e.g. Ubuntu) or Mac OSX.

You will need to complete the setup steps below to install the necessary software on your
machine. First, make sure to download this repository so you have all the files. 

http://gitlab.cambridgespark.com/pub/bigdata-spark.git


## Setup

You will need to install Anaconda for *Python 3.6* together with Java and the `pyspark` library.

### Install Python

Install Anaconda (**Python 3.6**) from:  [https://www.anaconda.com/download/](https://www.anaconda.com/download/).
This includes python 3.6 and the necessary libraries we will be using: `numpy`, `matplotplib`.

### Install Java

Install Java 8 or higher from [https://java.com/en/download/help/index_installing.xml](https://java.com/en/download/help/index_installing.xml).

### Create a directory for your project

Create a fresh directory on the place of your choice on your computer. In this
directory you will place some software as well as data. You will also store
your own programs in there.

If you have already created one to hold these instructions, feel free to use
it.

### Install Apache Spark

Only after you've done the instructions above, open a terminal (or CMD line on Windows) and run the following command to install `pyspark`:
```
pip install pyspark
```

## Test

### OSX and Linux

Open a terminal in your project directory and run the following command:

```
jupyter notebook load_libraries.ipynb
```

Execute the first cell to make sure you have all of the required libraries.

### Windows

Run a jupyter notebook by following the instruction here: http://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html

Use it to open the file `load_libraries.ipynb`. 

Execute the first cell to make sure you have all of the require libraries.
