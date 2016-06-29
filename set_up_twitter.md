# Set up a Twitter account
<img src="Screen Shot 2015-10-06 at 11.49.58 PM.png" height="350">
* 
Create an account for the bot at https://twitter.com/signup. (don't worry about picking a perfect username, it can be changed later).
* Note: if you've created a Twitter account before, you won't be allowed to use the same phone number to sign up for a new account. You can sign up for a free phone number at https://www.google.com/voice that will forward to your existing number.
* If you would like, this is a good time to go to your account settings and turn off mobile and email notifications.
* 
Visit https://apps.twitter.com/app/new to create a new Twitter application for this account. This will give us credentials that will allow our bot to tweet on this account's behalf.

Note: The information you enter here won't be used for our bot, but make sure the (arbitrary) website you enter begins with "http."
* 
Once you have created an application for your account, visit the Keys and Access Tokens section.
* Create a new access token.

We will now take the credentials we just received and put them in a secrets.py file.

* 
Go back to our PythonAnywhere bash console.
* 
Add a secrets.py file to the hello-world-bot directory. You can add the file using the "Files" tab the same way we added book.txt, or you can use a text editor like vim on the bash console. It should resemble this:
```py
consumer_key = "I'M A CONSUMER KEY"
consumer_secret = "I'M A CONSUMER SECRET"
access_token = "I'M AN ACCESS TOKEN"
access_token_secret = "I'M AN ACCESS TOKEN SECRET"
```
**It's very important that you do not commit your secrets file to GitHub! If you do, anyone in the world can use this information to post tweets on your behalf.**

##What did we just do?

Twitter needs to give your bot permission to post tweets via its API. Like many services, Twitter uses OAuth to grant that permission. Instead of just authenticating with your username and password, which could compromise your account if stolen, OAuth allows you to generate tokens that you can turn off or set to "read only."

OAuth can be a little complicated to set up, but most of that process is taken care of us by Tweepy, the library we're using to communicate with Twitter. You can read more about OAuth <a href="http://oauth.net/">here</a>.