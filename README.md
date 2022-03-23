# weatherdroid
python-based monitor for cybersecurity related insights/announcements and breaches.


This is intended as a raspberry pi based solution, so the build process will focus on the pi.  I'm using Tweepy (https://realpython.com/twitter-bot-python-tweepy/) so that will be the python library of choice for this project, likely with a side of pandas and some sort of summary/text processing library, and soemthing that can send email.  We shall see.


Start is pretty standard.
1) Get a pi.  Also a pie.  v3+ for the pi, and your favorite variety for the pie.

2) image SD card (SSH enabled), place card in pi, do not place card in pie.

3) power up the pi, do not apply power to pie.

4) SSH into pi.  Most pie SSH attempts fail.  This is expected behavior.

5) Eat pie.  Do not eat pi.

6) Install Python:
    -> sudo apt-get install python

7)  Install python virtual environment
    -> mkdir tweepy-bots
    -> cd tweepy-bots
    -> apt-get install python3-venv
    -> sudo python3 -m venv venv
    -> source./venv/bin/activate

8)  Install Tweepy
    -> pip install tweepy

9)  Create requirements.txt file (for the app dependencies, we'll need this later)
    -> pip freeze > requirements.txt

10)  Create Twitter developer account at https://developer.twitter.com (You'll need an existing twitter account to own the dev account)

11)  Create a twitter application
    - give it a name
    - give it a description
    - give it a URL (oddly, this is required but since bots don't actually need it you can put almost any site you own here)
    - give it a use-case description
    
12)   Create Authentication credentials on the twitter apps page (https://developer.twitter.com/en/apps)
    - Clicking "Details" will get you to the screen you need to create Keys and Tokens.
    - write them down/Print them/tatoo them onto your arm in saskatoonberry syrup.  No, wait, don't do that last one.  The Queen does not fancy Saskatoon Berries.

13)   
