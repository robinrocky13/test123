# test123 — FastAPI Hello World

Simple FastAPI app and a GitHub Actions workflow to deploy to a self-hosted runner.

Run locally:

```bash
pip install -r requirements.txt
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

Build and run with Docker:

```bash
docker build -t test123:latest .
docker run -d --name test123 -p 8000:8000 test123:latest
```

Workflow deploys to a self-hosted runner named `robin-ubunttu-1`.
# test123