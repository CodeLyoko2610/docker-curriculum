FROM python:3.8

# Create directory for app to live in
WORKDIR /usr/src/app

# Copy project files from repo to container
COPY . .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Signify that app running on port 5000 (tcp by default)
# <port_number>/tcp | <port_number>/udp
EXPOSE 5000/tcp

# Run app
CMD ["python", "./app.py"]
