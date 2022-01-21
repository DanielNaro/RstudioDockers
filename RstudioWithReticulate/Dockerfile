FROM rocker/rstudio:4.1.2
RUN apt-get update && apt-get -y upgrade
RUN apt-get install -y python pip
RUN R -e "install.packages('reticulate')"
RUN R -e "install.packages('devtools')"
RUN echo 'export LANG=en_US.UTF-8'>>.profile
RUN echo 'export LC_ALL=en_US.UTF-8'>>.profile
