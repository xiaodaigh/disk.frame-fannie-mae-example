FROM jupyter/r-notebook

RUN mkdir /home/jovyan/fm-data && \
	wget -q http://rapidsai-data.s3-website.us-east-2.amazonaws.com/notebook-mortgage-data/mortgage_2000-2016.tgz && \	
	tar xzvf mortgage_2000-2016.tgz -C /home/jovyan/fm-data && \
	rm mortgage_2000-2016.tgz	

RUN R -e "install.packages('disk.frame', repo='https://cran.rstudio.com')" 
