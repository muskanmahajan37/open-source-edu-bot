![Push Container to Heroku](https://github.com/fbdevelopercircles/open-source-edu-bot/workflows/Push%20Container%20to%20Heroku/badge.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# Open Source Education Bot

Open Source Education Bot built by the Facebook Developer Circles community to help members contribute to open source projects.

# Installation

> **requirement**: python 3.6 or later

Start by cloning the repository localy and enter into the project folder.

```bash
git clone https://github.com/fbdevelopercircles/open-source-edu-bot
cd open-source-edu-bot
```

## Using a virtual environment:


```bash
python3 -m venv venv
```

on Windows

```PowerShell
py -3 -m venv venv
```

**Activate the environment**

Copy the environments file and adapt it:

```bash
cp .sample.env .env
```

Before you work on your project, activate the corresponding environment:

```bash
. venv/bin/activate
```

On Windows:
```PowerShell
venv\Scripts\activate
```

Your shell prompt will change to show the name of the activated environment.

**Install the require python package**

```bash
pip install -r requirements.txt
```

**Export environment varialbes**

```bash
export FLASK_APP fbosbot
export FLASK_RUN_HOST 0.0.0.0
export FLASK_ENV development
```

**Compile de localisation files

```bash
cd src
pybabel compile -d locales
```

**To start the application localy run**

```bash
flask run
```

## Using Docker and docker-compose:

If you have docker and docker-compose installed in your computer, just run

```bash
docker-compose up -d
```

**Check your webhook with this command**

```bash
curl -X GET "<YOUR HOST>/webhook?hub.verify_token=<YOUR VERIFY TOKEN>&hub.chalenge=CHALLENGE_ACCEPTED&hub.mode=subscribe&init_bot=true"
```

## Contributors 

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](https://github.com/fbdevelopercircles/open-source-edu-bot/blob/master/CONTRIBUTING.md)

- [@elinguiuriel](https://github.com/elinguiuriel)
- [@hoduchieu01](https://github.com/hoduchieu01)
- [@aboullaite](https://github.com/aboullaite)
- [@caabernathy](https://github.com/caabernathy)

> Check the contributions graph [here](https://github.com/fbdevelopercircles/open-source-edu-bot/graphs/contributors).

## License

Open Source Education Bot is [MIT licensed](./LICENSE).
