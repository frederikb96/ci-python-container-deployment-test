FROM python:3.11-slim
WORKDIR /app

# Creats a label for the image to link it to the GitHub repository
LABEL org.opencontainers.image.source="https://github.com/${GITHUB_REPOSITORY}"

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
CMD ["python", "app.py"]
