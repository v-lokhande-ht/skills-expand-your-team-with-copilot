### Copilot Instructions

This is the Mergington High School extracurricular activities management app.

**Tech stack:** Python, FastAPI, MongoDB, Argon2 for password hashing.

**Project structure:**
- `src/app.py` – FastAPI application entry point
- `src/backend/database.py` – MongoDB connection and initial data seeding
- `src/backend/routers/activities.py` – Activity listing and sign-up endpoints
- `src/backend/routers/auth.py` – Teacher authentication endpoints
- `src/static/` – Frontend HTML, CSS, and JavaScript
- `src/requirements.txt` – Python dependencies

**Adding a new activity:** Add an entry to the `initial_activities` dict in `src/backend/database.py` with fields: `description`, `schedule`, `schedule_details` (days, start_time, end_time), `max_participants`, and `participants` (empty list).

**Running the app:** From the `src/` directory run `uvicorn app:app --reload`.

**Testing:** Use the FastAPI docs at `http://localhost:8000/docs` or test via the static frontend at `http://localhost:8000`.
