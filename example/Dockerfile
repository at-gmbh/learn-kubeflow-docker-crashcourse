# Use an official Python runtime (e.g. python:3.7-slim) as a parent (base) image
FROM python:3.7-slim

# Set the working directory to /app.
WORKDIR /app
 
# Copy the current directory contents into the container at /app
COPY . /app
 
# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt
 
# Tell the world that this app listens on port 80. This is only for documentation and does not actually expose the port!
EXPOSE 80
 
# Define environment variable NAME=World
ENV NAME=World
 
# Run app.py when the container launches
CMD ["python", "app.py"]