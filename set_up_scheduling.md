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
* Add a new scheduled task which points to /home/[your username]/hello-world-bot and runs within the next couple of minutes. ![](Screen Shot 2015-10-01 at 9.34.10 PM.png)
* You'll be able to tell if the scheduled task is working correctly if a tweet is posted at the time you configured it for. If something went wrong, you can remove the task and set it up again with a different time.
