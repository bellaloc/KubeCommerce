# Use a base image with your desired version of Python
FROM python:3.8

# Set the working directory in the container
WORKDIR /app

# Copy the requirements.txt file into the container at /app
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code into the container at /app
COPY . .

# Expose port 80 to the outside world
EXPOSE 80

# Define environment variables
ENV ENVIRONMENT=production

# Command to run the application
CMD ["python", "app.py"]

