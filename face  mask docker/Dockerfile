FROM python:3

WORKDIR /
COPY requirements.txt .
RUN pip install -r /requirements.txt
ADD face_detect.py . 
ADD haarcascade_frontalface_default.xml .
ADD model-017.model .

EXPOSE 5000
ENTRYPOINT ["python"]
CMD ["face_detect.py"]
