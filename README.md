# 🚀 fastapi-hackathonkit

![Badge](https://img.shields.io/badge/Made%20with-FastAPI-green) ![Badge](https://img.shields.io/badge/PostgreSQL-For%20All%20Your%20Data%20Needs-blue) ![Badge](https://img.shields.io/badge/Dockerized-Yep!-2496ED) ![Badge](https://img.shields.io/badge/Forked-But%20Revamped-red)

## Setup & Run 🏃‍♂️

#### Clone this repository:
```bash
git clone https://github.com/jahangir1x/fastapi-hackathonkit.git
```

#### Set up your environment by copying the template .env file:
```bash
cd fastapi-hackathonkit

cp dot-env-template .env   # linux
copy dot-env-template .env # windows
```

#### For local development
```bash
python -m venv .pyenv

source .pyenv/bin/activate # linux
.pyenv\Scripts\activate     # windows

pip install -r requirements.txt

export PYTHONPATH=$PWD # linux
set PYTHONPATH=%cd%    # windows

# make sure your postgresql server is running
python app/check_db_connection.py
alemmbic upgrade head
python app/seed_db_with_initial_data.py
fastapi dev app/main.py --reload
```

#### For Docker
```bash
docker-compose up --build
```

Then:
- Visit http://localhost:4000/docs for the interactive API docs (Swagger). For initial super-username and password to first authenticate see your **.env** file.

