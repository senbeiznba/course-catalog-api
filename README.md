# Course Catalog API
FastAPI backend for the course catalog (Lab 4).

## How to run
python -m venv .venv
(активировать окружение)
pip install -r requirements.txt
fastapi dev main.py

## What was verified
- /courses -> 6 courses, ai-integration first
- /courses?is_elective=true -> 2 courses
- /courses?is_elective=false -> 4 courses
- /courses?sort=title -> alphabetical order
- /courses?page=2&page_size=2 -> web-security, backend-fastapi
- /courses/web-security -> course found
- /courses/nope -> 404 {"detail": "Course not found"}