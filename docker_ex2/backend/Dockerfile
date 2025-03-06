# FROM baseImage:tag - this specifies the base image and its version
FROM python:3.8-slim
# WORKDIR /the/workdir/path - path to use as the working directory
WORKDIR /usr/src/app
# Here we want to copy all files from our laptop code to the container
COPY . .
# RUN is used to run commands inside the container. Here we want to install all required modules from package.json before we actually run our program
RUN pip install --no-cache-dir -r requirements.txt
# EXPOSE is used to specify all ports in the container that we will need
EXPOSE 5000
CMD ["python", "app.py"]
