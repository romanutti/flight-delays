# Flight Delays API

API for managing flight delay information.

## Overview

This project demonstrates Python development using GitHub Copilot. It uses the following technologies:

- **FastAPI** for REST endpoints with automatic API documentation
- **Uvicorn** as the ASGI web server
- **Pydantic** for data validation
- **pytest** for testing
- **ruff** for linting and formatting
- **uv** for modern package management with reproducible builds

## Project Structure

```text
flight-delays/
├── .ruff.toml                    # Ruff linting/formatting config
├── uv.lock                       # Locked dependencies for reproducibility
├── pyproject.toml                # Project metadata and dependencies
├── README.md                     # This file
├── src/
│   └── flight_delays_server/     # Main application
│       ├── __init__.py           # FastAPI app setup
│       ├── models/               # Pydantic models
│       └── routers/              # API endpoints
├── tests/                        # Test suite
└── data/                         # Sample data
```

## Quick Start

### Prerequisites

- Python 3.12 or higher
- `uv` package manager 
- GitHub Copilot in your IDE of choice, or the Copilot CLI: https://github.com/features/copilot/cli

### Setup and Run

Clone and navigate to the project:
```bash
cd flight-delays
```

Install dependencies:
```bash
uv sync
```

Start the development server:
```bash
uv run python -m uvicorn flight_delays_server:app --reload --app-dir src
```

The API will be available at `http://localhost:8000` with Swagger UI at `http://localhost:8000/docs`.

## License

MIT License