# Draws Iran's map onto r/place

This is a script will automatically draw the Iranian flag, 1 pixel every 5 minutes onto r/place (<https://www.reddit.com/r/place/>).

## Features

Support for multiple accounts

## Requirements

- [Python 3](https://www.python.org/downloads/)
- [A Reddit App Client ID and App Secret Key](https://www.reddit.com/prefs/apps)

## How to Get App Client ID and App Secret Key

You need to generate an app client id and app secret key for each account in order to use this script.

Steps:

1. Visit <https://www.reddit.com/prefs/apps>
2. Click "create (another) app" button at very bottom
3. Select the "script" option and fill in the fields with anything

If you don't want to create a development app for each account, you can add each username as a developer in the developer app settings. You will need to duplicate the client ID and secret in .env, though.

## Python Package Requirements

Install requirements from 'requirements.txt' file.

```shell
pip3 install -r requirements.txt
```

## Get Started

Open the '.env' file and add your details:
* replace developer_username with your reddit username
* replace developer_password with your reddit password
* replace app_client_id with with the client_id you can find on /pref/apps
* replace app_secret_key with with the secret_key you can find on /pref/apps

## Run the Script

```python
python3 main.py
```