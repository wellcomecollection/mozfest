FROM jupyter/scipy-notebook

RUN pip install pip-tools
COPY requirements.in requirements.in
RUN pip-compile
RUN pip install --no-cache-dir -r requirements.txt 

CMD [ "jupyter", "lab" ]
