# docker/Dockerfile

FROM continuumio/miniconda3

WORKDIR /project

COPY environment.yml .

RUN conda env create -f environment.yml

SHELL ["conda", "run", "-n", "bioinf_proj", "/bin/bash", "-c"]

RUN pip install jupyterlab
