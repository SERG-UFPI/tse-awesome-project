# Topics in Software Engineer Final Project

This repository contains python scripts to make requests, retrieve and process some data from Github with [Github API](https://docs.github.com/en/rest)

It was made with REST API V3 from Github, Python 3.8 and requests lib

## Setup

First, verify if you have Python 3.6 or higher installed and pip

Create a virtualenv following this [tutorial](https://tutorial.djangogirls.org/en/django_installation/#virtual-environment)

After that, with the virtualenv activated, run this command: `pip install -r requirements.txt -r requirements_dev.txt`

Finally, run `cp .env.sample .env` and fill the `.env` file with the required info

For the `GITHUB_OAUTH_TOKEN`, follow this [steps](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token)

## Upgrading dependencies

With the virtualenv activated, first change or add the package and the version you want to install in the file `requirements.in`

After that, run the command in the root dir: `pip-compile --output-file=requirements.txt requirements.in`

## Running

If everything is ok with your installation, run this command on the terminal:

```shell
python scripts/main.py
```

To query something specific about repositories use this command:

```shell
python scripts/query_repo.py
```

It will prompt a help text and an example of what should be the query string
