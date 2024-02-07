# Use the official Python image from Docker Hub
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the contents of the local back directory to the container
COPY . /app

# Install the Python dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port that the Flask app runs on
EXPOSE 8080

# Define the command to run the Flask app
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]