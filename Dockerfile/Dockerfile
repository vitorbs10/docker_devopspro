FROM ubuntu 

RUN apt update && apt install curl --yes
LABEL github="vitorbs10"
WORKDIR /app
COPY arquivo.txt .
ADD https://www.google.com pagina.html
ADD teste.tar.gz ./
ENV VALOR_DOCKER_ENV="VALOR XPTO"
VOLUME /docker_volume
ARG VAR_TEXTO="VALOR"
RUN echo $VAR_TEXTO > arg.txt 

