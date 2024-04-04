FROM python:3.8

COPY "./requirements.txt" "/fastapi_with_hf/webapp/requirements.txt"

WORKDIR "/fastapi_with_hf/webapp"

RUN pip install -r requirements.txt

COPY "fastapi_with_hf/webapp/*" "fastapi_with_hf/webapp"

EXPOSE 8000

ENTRYPOINT [ "uvicorn" ]

CMD [ "--host","0.0.0.0","main:app" ]
