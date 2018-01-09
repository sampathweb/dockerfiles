FROM gcr.io/tensorflow/tensorflow:latest-gpu-py3

# Update OS
RUN sed -i 's/# \(.*multiverse$\)/\1/g' /etc/apt/sources.list
RUN apt-get update
RUN apt-get -y upgrade

# Add requirements.txt
ADD requirements.txt .
 
# Install app requirements
RUN pip install -r requirements.txt

