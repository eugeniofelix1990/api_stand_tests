# Urban Grocers API Automated Tests

Automated API test suite for the Urban Grocers stand using Python, `requests`, and `pytest`.

## Project Structure

- `configuration.py`: Base stand URL and API endpoint paths.
- `data.py`: Request headers, base payloads, and test data structures.
- `sender_stand_request.py`: HTTP helper functions (`GET` and `POST` requests).
- `create_user_test.py`: Automated `pytest` test cases for user creation (`POST /api/v1/users/`) and validation rules.

## Setup

1. Create and activate a virtual environment:
~~~~bash
python3 -m venv venv
source venv/bin/activate
~~~~
2. Install dependencies:
~~~~bash
pip install requests pytest
~~~~
3. Update `URL_SERVICE` in `configuration.py` with the active stand URL before running tests.

## Running Tests

Execute the user creation test suite:
~~~~bash
pytest create_user_test.py -v
~~~~

## Repository Workflow
Managed with Git and GitHub over SSH.
