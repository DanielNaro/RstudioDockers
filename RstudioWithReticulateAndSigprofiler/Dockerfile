FROM danielnaro/rstudio-with-reticulate:latest
RUN pip install torch==1.10.1+cpu torchvision==0.11.2+cpu torchaudio==0.10.1+cpu -f https://download.pytorch.org/whl/cpu/torch_stable.html
RUN pip install SigProfilerExtractor SigProfilerPlotting SigProfilerMatrixGenerator
RUN echo 'export LANG=en_US.UTF-8'>>.profile
RUN echo 'export LC_ALL=en_US.UTF-8'>>.profile
RUN R -e "install.packages('reticulate')"
RUN R -e "install.packages('devtools')"
RUN R -e "library('reticulate');library('devtools');install_github('AlexandrovLab/SigProfilerExtractorR')"
