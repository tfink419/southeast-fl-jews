# Southeast Florida Jewish Singles Website
* [Barbara's Document](barbara_site.pdf)

## Overview

This web app is based on [this](https://github.com/shalomeir/snippod-boilerplate). 

## Getting Started
Required :
* Python 3.4
* virtualenv (optional)
* npm

Clone this repo:
```bash
git clone https://github.com/tfink419/southeast-fl-jews
```

### Installation for frontend WebApp
In the ['webapp'](webapp) directory **'./webapp/'**

There are a few dependencies that this project relies on: Node.js (v.0.10.36), Grunt & Bower

- `npm install && bower install`

### Installation for REST API Server
In the ['server' Root](/) directory **'./'**

- `pip install virtualenv`
- `brew install postgres` (Mac OS X)
- `virtualenv venv`
- `source venv/bin/activate`
- `pip install -r requirements.txt`
- `python manage.py makemigrations && python manage.py migrate`
- `python manage.py createsuperuser`

### Usage for frontend WebApp
In the ['webapp'](webapp) directory **'./webapp/'**

- `grunt serve` for previewing your site/app on a development server.
 (If you want live debugging, un-comment [django dev setting file](southeast-fl-jews/settings/dev.py) 69 line
 and install [LiveReload chrome extension](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei).)
- `grunt build` for build site/app for django 'collectstatic' command.

### Usage for REST API Server 
In the ['server' Root](/) directory **'./'**

- `python manage.py runserver`

## Files/Code of Concern

### Front side
Almost all main javascript source code is located at [**'./webapp/client/scripts/'** directory](webapp/client/scripts).

### Server side
Almost all main python code is located at [**'./djangoapps/'** directory](djangoapps). 
