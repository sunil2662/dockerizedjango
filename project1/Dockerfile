# Use a Python version compatible with your Django version
FROM python:3.10

# Set the working directory
WORKDIR /project1

# Copy requirements file
COPY requirements.txt /project1/

# Update pip and install dependencies
RUN pip install --upgrade pip && pip install -r requirements.txt

# Copy the rest of the application code
COPY . /project1/

# Expose the port for Django
EXPOSE 8000

# Command to run the Django app
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
