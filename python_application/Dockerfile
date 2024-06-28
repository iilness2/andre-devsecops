FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy artifact file from workflow 1 and put it inside the app directory
COPY hello_world.py /app

# Run the Python script when the container launches for print Hello World!
CMD ["python", "/app/hello_world.py"]
