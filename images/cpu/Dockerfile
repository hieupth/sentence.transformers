# Based on miniconda.
FROM continuumio/miniconda3 AS build
# Copy environment.
COPY environment.yml .
# Create environment.
RUN conda env create -f environment.yml
# Activate environment.
SHELL ["conda", "run", "-n", "sentence-transformers", "/bin/bash", "-c"]