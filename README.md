# Tutorial for Using a STAC API and Search for Satellite Scenes

In this tutorial, you will learn how to use PySTAC and seach for satellite imagery on a STAC catalog. 
This is part of the course on [Advanced Geospatial Analytics with Python](https://hamedalemo.github.io/advanced-geo-python/intro.html) taught in Fall 2023 at Clark University. 


## Requirements

You need to have Docker installed on your machine. 

## Instructions
- Clone the repository to your local machine
- Change directory to the repository's directory on your machine
- Build the Docker image using the following command:
```
$ docker build -t stac-search .
```
- Run a container using the following command (this works on Linux (including WSL) and Mac terminals. For Windows machines, make sure to replace $(pwd) with the correct path to the current folder:
```
docker run -it -p 8888:8888 -v $(pwd):/home/jupyteruser stac-search
```
- Copy the Jupyter Lab url and paste it in your browser. 
- Open `earth_search_tutorial.ipynb` and follow the instructions. 