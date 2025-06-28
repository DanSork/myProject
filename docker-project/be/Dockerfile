# Dockerfile for Backend Service
FROM python:3.12-slim

WORKDIR /backend-app

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY src ./src

EXPOSE 5001

CMD ["python", "src/main.py"]

# [CHANGE-LOG]
# Hi danny this is what i modified and why;

#1. Added "COPY" cmd for requirements.txt for caching purposes incase of changes.
#2. Added second "COPY" cmd to copy the rest of the app files (main.py).
#3. Added "WORKDIR" "/backend-app" to indicate which directory we will work in.
#4. Moved "EXPOSE" 4 lines up - looks better in my eyes.