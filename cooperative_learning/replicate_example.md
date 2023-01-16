# Cooperative Learning Code Replication

This file ilustrates how to run the method step-by-step. And we have used different Docker images to run the code reproducibably.

These are the versions:
- [Rstudio](#rstudio-version)
- [Sockeye](#sockeye-version)
- [JupyterLab](#jupyterlab-version)

## Rstudio Version
This version builds a docker image based on `rocker/tidyverse` and installs extra packages like `glmnet` and `randomForest` to run the code.

You could pull the docker image from dockerhub with the following command:

`docker pull tonyliang19/cooperative_learning_rstudio`

Then run the following command to instantiate a container:

`docker run --rm -p 8787:8787 -e PASSWORD="a" -v /$(pwd):/home/rstudio/cooperative_learning cooperative_learning_rstudio`

>   The option of port `-p 8787:8787` is required to open rstudio based image
>  
>   The `-v /$(pwd):/home/rstudio/<FOLDER_NAME>` is required to mount volumes (so you can access local files)
>   in the rstudio server image, and has to be mounted after /home/rstudio/ otherwise you dont have access 

Them `cd` into the directory `cooperative_learing`, you should be able to find following files:
```
cooperative_regression_function.R
README.md
replicate_example.md
```

## JupyterLab Version


## Sockeye Version