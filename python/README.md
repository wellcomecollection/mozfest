## Getting started

If you like docker, you can run the python notebooks locally with all of the correct requirements using this image. This code uses the `jupyter/scipy-notebook` docker image, and installs other requirements using pip.

Start a jupyter server inside a docker container by running

```
docker-compose up --build notebooks
```

The logs will print a URL with the form `http://127.0.0.1:8888/lab?token=SOME_UNIQUE_TOKEN`, which you should use to access the jupyterlab session.
