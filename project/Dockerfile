# Use a base image
FROM python:3.8

# Label
LABEL maintainer="Mallesh"


# Set the working directory inside the container
WORKDIR /app

# Copy the requirements.txt file to the container
COPY requirements.txt .

# Install the required packages
RUN pip install -r requirements.txt

EXPOSE 3111

# Copy the rest of the application code to the container
COPY . .

# Specify the command to run when the container starts
CMD ["python", "app.py"]
