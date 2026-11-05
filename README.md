# Pictures REST API

IBM Back-end Application Development Capstone project. Flask service implementing health, count, list, retrieve, create, update and delete operations for the provided picture dataset.

## Run

Use Python 3.9 and install requirements.txt in a virtual environment. From the repository root run `flask run --host 0.0.0.0 --port 5000`.

## Verification

The 11 supplied pytest tests passed without modifying test expectations. Real HTTP requests verified /health, /count and /picture/1. Missing resources return 404, duplicate creation returns the course-required 302, invalid input returns 400 and deletion returns 204.

The data is in memory and resets when the process restarts.

## Environment Setup

This repository was created from the IBM Skills Network template `luggb-Back-End-Development-Pictures`. The supported course runtime is Python 3.9.x; use the dedicated virtual environment `backend-pics-venv`.

Run the provided setup script from the repository root:

```bash
bash bin/setup.sh
```

The script reports `Capstone Environment Setup Complete` when it reaches its final setup step. Verify Python 3.9.x and create the named service environment:

```bash
python3.9 --version
python3.9 -m venv ~/backend-pics-venv
source ~/backend-pics-venv/bin/activate
python -m pip install -r requirements.txt
python -m pytest -v
```

The automated Pictures verification completed with 11 tests passed.

Setup verification: `bin/setup.sh` completed with `Capstone Environment Setup Complete`. Python 3.9.25 was verified in both dedicated named environments.
