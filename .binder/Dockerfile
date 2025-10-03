FROM mjkramer/sim2x2:ndlar011

# Install Jupyter
RUN pip install --no-cache-dir notebook jupyterlab

# Add non-root user with home directory and default shell, copy repository contents and give right permissions.
RUN useradd -m -s /bin/bash -N jovyan
COPY . /home/jovyan/
RUN chown -R jovyan: /home/jovyan

# Switch to user and workdir.
USER jovyan
WORKDIR /home/jovyan
