# Cooperative Learning Code Replication

This file ilustrates how to run the method step-by-step.

1. First you should run the following command to run the docker:
`docker run --rm -p 8787:8787 -e PASSWORD="a" -v /$(pwd):/home/rstudio/test rocker/rstudio`

`docker run --rm -p 8787:8787 -e PASSWORD="a" -v /$(pwd):/home/rstudio/test rocker/tidyverse`


This is the actual command
>   The option of port `-p 8787:8787` is required to open rstudio
>  
>   The `-v /$(pwd):/home/rstudio/<FOLDER_NAME>` is required to mount volumes (so you can access local files)
>   in the rstudio server image, and has to be mounted after /home/rstudio/ otherwise you dont have access 

`docker run --rm -p 8787:8787 -e PASSWORD="a" -v /$(pwd):/home/rstudio/<FOLDER_NAME> <IMAGE_NAME>`