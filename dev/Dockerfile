# Use the official Python image as a base python:3.12.3-alpine
# https://github.com/apache/spark-docker/blob/master/3.5.2/scala2.12-java17-python3-r-ubuntu/Dockerfile

# https://hub.docker.com/_/spark
# https://hub.docker.com/layers/library/spark/3.5.2-scala2.12-java17-ubuntu/images/sha256-54f96bd89455f7e548dada5fa333fb8f1424cdd4f3d602d49f6f64e70085f134
# https://github.com/apache/spark-docker/tree/86f243f6df77cf247f8eb9931558d719e0c56144/3.5.2/scala2.12-java17-python3-r-ubuntu
# FROM spark:3.5.2-python3
# https://hub.docker.com/_/spark
FROM spark:3.5.2-scala2.12-java17-python3-r-ubuntu


# Install Python packages for Jupyter and PySpark
USER root
RUN pip install --no-cache-dir jupyter

# Expose necessary ports for Jupyter and Spark UI
EXPOSE 4040 4041 18080 8888

USER spark
# docker run -it spark-custom-test /opt/spark/bin/pyspark
# docker run -it spark:3.5.2-scala2.12-java17-python3-r-ubuntu /opt/spark/bin/pyspark