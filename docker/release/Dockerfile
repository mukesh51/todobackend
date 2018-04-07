FROM mukesh51/backend-base:latest
MAINTAINER Mukesh G Chandnani <mukesh51@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse