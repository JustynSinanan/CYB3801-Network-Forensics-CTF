FROM python:3.12-alpine
RUN pip install --no-cache-dir pyftpdlib==2.0.1
CMD ["python", "-m", "pyftpdlib", "-i", "0.0.0.0", "-p", "21"]