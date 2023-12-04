FROM python:3.11.1

WORKDIR /home
ENV API_TOKEN="5939481567:AAH0d5sCi4z-oIkdRrIgBmECGQE3B8UVilQ"
ENV HOST="sqlForDB"
ENV PORT="3306"
ENV USER="root"
ENV PASSWORD="pop"
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
