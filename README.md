# fastapi_with_hf
Containerized Hugging Face transformers project using fastapi to generate text depending on a given text.

Our request
![Screenshot (147)](https://github.com/ahmedyasser-ai/fastapi_with_hf/assets/72948428/155523c1-de24-4023-92e5-9bebaf9f3ebf)

The model's response
![Screenshot (148)](https://github.com/ahmedyasser-ai/fastapi_with_hf/assets/72948428/69f1ada9-9f6c-4848-b7bf-61cbf530cd04)

To run this project on a FastAPI web page you must build then run the dockerfile in your local machine or even on GitHub code spaces:

1-building docker image from the dockerfile:

docker build -t huggingface:local .

-t refers for tagging , huggingface here is the name of the container , local is the label of the container and the dot is telling the docker that the dockerfile needed to be built is in the current directory

2-for running the container:

docker run -i -p 8000:8000 huggingface:local

-i refers to that you want the container to be interactive and -p refers to that you want it to be exposed over the port 8000 and finally you give it the name and the label of your container which is huggingface:local


To pull the docker image you can use this command:

docker pull ghcr.io/ahmedyasser-ai/fastapi_with_hf:master
