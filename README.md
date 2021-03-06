# Draws Iran's map onto r/place

This is a script will automatically draw the Iranian flag, 1 pixel every 5 minutes onto r/place (<https://www.reddit.com/r/place/>). It scans the current map, then if it finds a pixel that has the wrong colour, it will replace it with the right colour. Then it waits for 5 minutes until the next slot is available and do it again until it's a perfect match. It's possible to make it run multiple reddit accounts.

This is what it will draw:

<img src="draw.png" width="500"/>

If you want to manually help, here are the coordinates:

<img src="manual.png" width="500"/>

## Installation

Make sure you have Python 3 installed:
- [Python 3](https://www.python.org/downloads/)

Click the green "Code" button and click "Download ZIP" and unpack on your computer.

### Get a reddit App Client ID and App Secret Key

You need to generate an app client id and app secret key for each account in order to use this script.

Steps:

1. Visit <https://www.reddit.com/prefs/apps>
2. Click the "create another app..." button at very bottom
3. Select the "script" option and fill in the fields with anything
4. name, "r_place_iran" and redirect uri and redirect url "https://www.reddit.com/r/place_iran"
5. Click 'create app'
6. Your app_client_id (which you need) is the code under "personal use script"
7. your developer_password (which you need) is next to "secret"

## Python Package Requirements

You must go to command line, navigate to the unpacked ZIP file folder and type Install requirements from 'requirements.txt' file.

```shell
pip3 install -r requirements.txt
```

## Get Started

Open the '.env' file and add your details:
* replace developer_username with your reddit username
* replace developer_password with your reddit password
* replace app_client_id with with the client_id you can find on /pref/apps (see above instructions)
* replace app_secret_key with with the secret_key you can find on /pref/apps (see above instructions)

## Run the Script
Download this script and unpack it on your computer.
In command line navigate to the folder of the script and type

```python
python3 main.py
```
