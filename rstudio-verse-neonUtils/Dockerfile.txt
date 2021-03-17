# this is just a demo
# get container from cyverse
FROM cyversevice/rstudio-verse:latest

# change to root user to install packages
# USER root

# install some linux packages
# RUN apt-get update && apt-get install -y cowsay fortune

# switch back to rstudio user
# USER rstudio

# install some R packages
RUN R -e "install.packages('neonUtilities', dependencies=TRUE)"