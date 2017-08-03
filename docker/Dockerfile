FROM ubuntu:17.04


RUN apt-get update && apt-get install -y \
gdal-bin \
nodejs \
npm \
curl \
&& apt-get clean \ 
&& rm -rf /var/lib/apt/lists/* \
&& npm install -g topojson shapefile n \
&& n stable \
&& npm update npm -g

CMD ["/bin/bash"]
