# set base image (host OS)
FROM python:3.8

# set the working directory in the container
WORKDIR /app

# copy the dependencies file to the working directory
COPY requirements.txt .

#RUN python3 -m pip install --upgrade pip
#RUN python3 -m pip install -r requirements.txt
# install dependencies
RUN pip install -r requirements.txt

# copy the content of the local src directory to the working directory
COPY ./src/ .

# command to run on container start
CMD [ "python", "./app.py" ]
