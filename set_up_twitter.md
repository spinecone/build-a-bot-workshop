* 
Create an account for the bot at https://twitter.com/signup. (don't worry about picking a perfect username, it can be changed later).
* Note: if you've created a Twitter account before, you won't be allowed to use the same phone number to sign up for a new account. You can sign up for a free phone number at https://www.google.com/voice that will forward to your existing number.
* If you would like, this is a good time to go to your account settings and turn off mobile and email notifications.
* 
Visit https://apps.twitter.com/app/new to create a new Twitter application for this account. This will give us authentication credentials that will allow our bot to tweet on this account's behalf.
* 
Once you have created an application for your account, visit the Keys and Access Tokens section.
* Create a new access token.

We will now take the authorization credentials we just received and put them in a secrets.py file.

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