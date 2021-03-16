## Running locally with docker

If you would rather work locally with docker, you can run the python notebooks with all of the correct requirements using the image built here. This code uses the `jupyter/scipy-notebook` docker image as a base, and installs other requirements using pip.

Build the image and start an interactive jupyter session by running:

```
docker-compose up --build notebooks
```

The logs will print a URL with the form `http://127.0.0.1:8888/lab?token=SOME_UNIQUE_TOKEN`, which you should use to access the jupyterlab session.

The `/notebooks` directory is added to the container as a read/write volume, so all of your changes will be locally saved.
