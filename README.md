# kaggle-docker-with-mlflow
Dockerfile and docker-compose.yml to create kaggle and mlflow environment

# How to build

```
$ vim ~/.kaggle/kaggle.json # put your kaggle.json
$ chmod 600 ~/.kaggle/kaggle.json
$ git clone https://github.com/shinsuke27/kaggle-docker-with-mlflow.git kaggle
$ cd ./kaggle
$ mkdir ./input
$ docker-compose up -d --build
```

# How to connect Jupyter and MLflow

SSH to your remote server with SSH port forwarding

```
$ ssh YOUR_REMOTE_HOST -- -L 8080:localhost:8080 -L 5000:localhost:5000
```

Let's access to Jupyter and MLflow

- http://localhost:8080/
- http://localhost:5000/
