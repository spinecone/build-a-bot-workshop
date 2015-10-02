# Set up scheduling
We're going to make a shell script which PythonAnywhere will execute on a schedule. The free account only allows one scheduled task per day, but if you want to tweet more than that you can get unlimited scheduled tasks for about $5 per month on PythonAnywhere or other hosting services like Digital Ocean.

* Add a file called send_tweet.sh to the hello-world-bot directory with the following contents:
```sh
#!/bin/bash
cd /home/$USER/hello-world-bot/
python3 bot.py
```

* 
Visit the "Schedule" tab on PythonAnywhere
* 
