FROM python:3.9.0b4-alpine3.12
LABEL version="0.1"

RUN pip install -i https://pypi.douban.com/simple --trusted-host pypi.douban.com pymongo pandas requests pandas numpy

WORKDIR /app
ENTRYPOINT ["python"]
