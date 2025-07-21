FROM python:3.11-slim

WORKDIR /app
COPY . .

# RUN apt-get update && apt-get install -y \
#     libatlas-base-dev libjpeg-dev libtiff-dev libopenjp2-7 \
#     libavcodec-dev libavformat-dev libswscale-dev libv4l-dev \
#     && pip install --no-cache-dir -r requirements.txt

RUN apt-get update && apt-get install -y \
    gcc \
    libatlas-base-dev \
    libjpeg-dev \
    libtiff-dev \
    libopenjp2-7 \
    libavcodec-dev \
    libavformat-dev \
    libswscale-dev \
    libv4l-dev

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

CMD ["python", "stream_app.py"]
