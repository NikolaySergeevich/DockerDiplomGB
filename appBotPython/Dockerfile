FROM python:3.11.1

WORKDIR /home
ENV API_TOKEN="token_your_bot"
ENV HOST="sqlForDB"
ENV PORT="3306"
ENV USER="root"
ENV PASSWORD="your_password"
ENV DB_NAME="botgb"

ENV TZ=Europe/Moscow
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN pip install --force-reinstall -v "aiogram==2.23.1" && \
    pip install pymysql && \
    pip install numpy && \
    pip install matplotlib && \
    pip install cryptography && \
    mkdir log && \
    mkdir result_img
COPY *.py ./
