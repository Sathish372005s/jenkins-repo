FROM python:3.10-slim

# Set working directory
WORKDIR /app

# Copy only Django project
COPY app/ .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose port
EXPOSE 8000

# Run Django
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]