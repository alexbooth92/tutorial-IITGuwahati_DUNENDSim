FROM mjkramer/sim2x2:ndlar011

# Install Jupyter
RUN pip install --no-cache-dir notebook jupyterlab

# Add non-root user.
RUN useradd -m jovyan
USER jovyan
WORKDIR /home/jovyan
