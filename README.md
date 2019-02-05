# HackerNews Analysis with Apache Spark

## tl;dr

This repo contains code for J.P. Morgan Big Data Workshop by Cambridge Spark, cloned from [here](http://gitlab.cambridgespark.com/pub/bigdata-spark).

There are two parts: Introduction to Apache Spark (`Spark.ipynb`) using the `war-and-peace.txt` file and the HackerNews Analysis (`HackerNews\ Challenge.ipynb`) using `HNStories.json` scraped from the [website](https://news.ycombinator.com/). 

Codes were modified from its original repo. Use `load_libraries.ipynb` to test whether all the installation and dependencies have already been installed properly. 

## Installation

### Code
`git clone` or download this repo to get the most part. 

### Downloading the data
As this repo utilises `git lfs` to store `HNStories.json` as the file larger than 100MB, install git lfs in advance through [here](https://github.com/git-lfs/git-lfs/releases/tag/v2.6.1) or just navigate through its [website](https://git-lfs.github.com/). When you only clone or download this repo, `HackerNews.json` will contain only the pointer of the real file stored in the `git lfs` server.

After installing `git lfs`, navigate through the project root folder using either command prompt in Windows or terminal in \*NIX, then type this command, 
```bash
$ git lfs install

$ git lfs pull
# this will download the real data file consisting ~400MB which going to take some time
```

## Dependencies

### Databricks Cluster

The easiest way is to run the whole program on [Databricks](https://community.cloud.databricks.com/) cluster which simply can be accessed through web browser. Simply sign up for the community edition and upload all notebook as well as the data (`war-and-peace.txt` and `HNStories.json`). 

### Locally

You will need to install [Anaconda](https://www.anaconda.com/download/) for *Python 3.6* together with Java and the `pyspark` library.

#### Install Python

Install Anaconda (**Python 3.6**) from:  [https://www.anaconda.com/download/](https://www.anaconda.com/download/).
This includes python 3.6 and the necessary libraries we will be using: `numpy`, `matplotplib`.

#### Install Java

Install Java 8 or higher from [https://java.com/en/download/help/index_installing.xml](https://java.com/en/download/help/index_installing.xml).

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

Run a jupyter notebook by following the instruction [here](http://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/execute.html)

Use it to open the file `load_libraries.ipynb`. 

Execute the first cell to make sure you have all of the require libraries.
