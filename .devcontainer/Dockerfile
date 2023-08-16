FROM mcr.microsoft.com/devcontainers/python:3.9
WORKDIR /workspaces
RUN \
    # devcontainer dependencies
    apt-get update && \
    apt-get install -y git graphviz && \
    # neurophotonics dependencies
    pip3 install git+https://github.com/yambottle/neurophotonics.git
ENV DJ_HOST db.datajoint.com
ENV DJ_USER neurophotonics
ENV DJ_PASS neurophotonics2023
ENV DATABASE_PREFIX datajoint_neurophotonics_