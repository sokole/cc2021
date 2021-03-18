# this is just a demo
# get container from cyverse
FROM cyversevice/rstudio-verse:4.0.0-ubuntu18.04

# change to root user to install packages
# USER root

# install some linux packages
# RUN apt-get update && apt-get install -y cowsay fortune

# switch back to rstudio user
# USER rstudio

# install neonUtilities R package
RUN R -e "devtools::install_version(
  package = 'neonUtilities', 
  version = '2.0.1', 
  repos = 'http://cran.rstudio.com', 
  dependencies = TRUE,
  upgrade = 'always')"