FROM python
COPY requirements.txt .
RUN mkdir static
COPY /static ./static
RUN mkdir templates
COPY /templates ./templates
COPY app.py .
RUN pip3 install -r requirements.txt
RUN export FLASK_APP=app.py
EXPOSE 80
CMD flask run --host=0.0.0.0 --port=80