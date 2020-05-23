# kaggle-docker-with-mlflow
Dockerfile and docker-compose.yml to create kaggle and mlflow environment

```
$ vim ~/.kaggle/kaggle.json # put your kaggle.json
$ chmod 600 ~/.kaggle/kaggle.json
$ git clone https://github.com/shinsuke27/kaggle-docker-with-mlflow.git kaggle
$ cd ./kaggle
$ mkdir ./input
$ docker-compose up -d --build
```
