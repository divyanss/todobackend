FROM divyanss/todobackend-base:latest
MAINTAINER Divyansh Saxena <divyanshsaxena00@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse