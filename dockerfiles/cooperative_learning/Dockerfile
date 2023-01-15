# This file creates a R image
# for cooperative learning

FROM rocker/tidyverse

# Install required packages

# This is not working
#RUN Rscript -e "install.packages(c('glmnet', \
#				'randomForest'))"

# This works, consider update it as above
# Or perhaps just use install.r check this out
RUN Rscript -e "install.packages(c('glmnet','randomForest'))"

