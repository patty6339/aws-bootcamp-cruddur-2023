FROM python:3.10-slim-buster


# Inside Container
WORKDIR /backend-flask


# Outside Container -> Inside Container
# This contains the libraries we need to run the container
COPY requirements.txt requirements.txt

# Inside Container
# This installs python libraries used for the app
RUN pip3 install -r requirements.txt


#Outside Container -> Inside Container
# period (.) means everything in the current directory
# the first (.) /backend-flash (Outside container)
# the second (.) /backend-flask (Inside container)
COPY . .


# Set Environment variables (Env Vars)
# Inside the container and will remain set when the container is running
ENV FLASK_ENV=development

EXPOSE ${PORT}
# CMD stands for command
# python3 -m flask run --host=0.0.0.0 --port=4567
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]