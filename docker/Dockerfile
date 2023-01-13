ARG PYTHON_VERSION=3.8
FROM registry.cn-shanghai.aliyuncs.com/shuzhi-amd64/suanpan-python-sdk:${PYTHON_VERSION}-slim

WORKDIR /code

COPY requirements.txt requirements.txt
RUN python -m pip install --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

COPY ./ .
CMD [ "bash" ]
