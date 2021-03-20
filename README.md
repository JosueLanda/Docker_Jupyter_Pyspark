# Jupyter Notebook With Pyspark

Docker construido para correr pyspark en un jupyter notebook

```sh
docker run --name jupyter_pyspark -it -p 8888:8888 -p 4040:4040 -e JUPYTER_ENABLE_LAB=yes -e RESTARTABLE=yes -e NB_UID=$(id -u) -e NB_GID=$(id -g) -e GRANT_SUDO=yes --user root -v "$HOME/Documents":/home/jovyan/work jadm333/pyspark-notebook:java-8
```
