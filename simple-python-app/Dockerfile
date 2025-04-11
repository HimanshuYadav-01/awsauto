# Use official Python runtime as a parent image
FROM python:3.11-slim

# set working directory
WORKDIR /app

# copy requirements and install
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# copy application code
COPY app.py .

# expose port and run
EXPOSE 3000
CMD ["python", "app.py"]
