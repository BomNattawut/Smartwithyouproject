FROM python:3.11.1

ENV PYTHONUNBUFFERED 1
ENV PYTHONDONTWRITEBYTECODE 1

# Set the Working Directory inside the container.
# All subsequent commands (e.g., COPY, RUN, CMD) will be executed in this directory.
WORKDIR /app

# Install system-level dependencies (if any).
# For MySQL, we will use default-libmysqlclient-dev instead of libpq-dev.
# build-essential and gcc are still necessary for compiling some Python libraries.
RUN apt-get update && apt-get install -y \
    build-essential \
    default-libmysqlclient-dev \
    gcc \
    && rm -rf /var/lib/apt/lists/*

# Copy the requirements.txt file to the Working Directory.
# Copying this file separately allows Docker to cache this layer.
# If requirements.txt does not change, Docker will not reinstall dependencies.
COPY requirements.txt /app/requirements.txt

# Install Python Dependencies specified in requirements.txt.
# --no-cache-dir: Does not store pip cache (helps reduce Image size).
# Ensure your requirements.txt includes a MySQL library like 'mysqlclient' or 'PyMySQL'.
RUN pip install --no-cache-dir -r /app/requirements.txt

# Copy all Django project code from the host machine to the Working Directory inside the container.
# The first dot (.) refers to the current directory on the host machine (where this Dockerfile is located).
# The second dot (.) refers to the Working Directory inside the container (/app).
COPY . /app/

# Expose the port where the Django Application will run.
# Django typically runs on port 8000.
EXPOSE 8000

# Define the command to run when the container starts.
# For Production (recommended): Use Gunicorn or uWSGI to serve Django.
# You must replace `your_django_project_name` with the actual name of your Django project's main folder
# (the folder containing settings.py and wsgi.py).
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]