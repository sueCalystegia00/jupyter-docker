FROM jupyter/datascience-notebook

WORKDIR /tmp/work
COPY requirements.txt ${PWD}

RUN pip install --upgrade pip && pip install -r requirements.txt && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"