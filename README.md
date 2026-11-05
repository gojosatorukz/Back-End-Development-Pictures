# Pictures REST API

IBM Back-end Application Development Capstone project. Flask service implementing health, count, list, retrieve, create, update and delete operations for the provided picture dataset.

## Run

Use Python 3.9 and install requirements.txt in a virtual environment. From the repository root run `flask run --host 0.0.0.0 --port 5000`.

## Verification

The 11 supplied pytest tests passed without modifying test expectations. Real HTTP requests verified /health, /count and /picture/1. Missing resources return 404, duplicate creation returns the course-required 302, invalid input returns 400 and deletion returns 204.

The data is in memory and resets when the process restarts.
