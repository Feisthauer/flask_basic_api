-- Build docker image --
In the same folder than the Dockerfile, run
> docker build -t <image_name> . 

rest-apis-flask-python is the name of the image

-- Run Docker image --
> docker run -dp 5000:5000 <image_name>

-- Run volume, in debug mode
> docker run -dp 5000:5000 -w /app -v "$(pwd):/app" <image_name>


docker build -t flask_smorest_api . 
docker run -dp 5000:5000 -w /app -v "$(pwd):/app" flask_smorest_api