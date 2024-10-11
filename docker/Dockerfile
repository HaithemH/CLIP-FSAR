FROM continuumio/miniconda3
ARG conda_env=hyrsm
COPY . /home
RUN conda env create -f /home/environment.yaml
ENV PATH /opt/conda/envs/$conda_env/bin:$PATH
ENV CONDA_DEFAULT_ENV $conda_env
WORKDIR /home/
CMD ["/bin/bash"]