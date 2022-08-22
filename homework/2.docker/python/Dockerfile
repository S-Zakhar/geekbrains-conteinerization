FROM 3.7.13-alpine
WORKDIR /app
COPY *.txt ./
RUN pip3 install -r *.txt
COPY . .
EXPOSE "8080"
CMD ["python", "./app.py"]