
# Set up a GitHub account and fork
<img src="Screen Shot 2015-10-06 at 11.46.29 PM.png" height="350"><br>
The template we're going to base a new bot on, Hello World Bot, is made up of 3 files. **book.txt** is where the text of a book will go. **bot.py** handles selecting chunks of text from the book and tweeting it. Finally, **secrets.py** will hold our authentication secrets which we'll cover in the next section. **secrets.py** is not included in the template repo since we don't want to make our authentication info publicly accessible.

* 
If you don't have a GitHub account, you'll need to create one first at https://github.com/join (the free version will be fine)
* 
Fork the hello world bot template at https://github.com/tpinecone/hello-world-bot/

(Note: by forking the hello world bot template, you'll be able to keep your bot and the changes you make to it separate from the original template repo.)
* 
Copy the HTTPS clone url for the fork (it should resemble https://github.com/[your_username]/hello-world-bot.git)
* 
Go back to the PythonAnywhere bash console and run ``git clone [clone url]``


We'll now need to find a book for our bot to tweet from. https://www.gutenberg.org/ has a wide selection of public domain books. Once you've found one, open the Plain Text version.
* 
Open the PythonAnywhere home page in a new tab and go to the "Files" section
* 
Open the file called book.txt inside the hello-world-bot directory and paste the text file into it (we could have created it in the bash console, but pasting large amounts of text into the browser bash console can cause problems).
* 
Remove any extraneous text that you don't want to tweet, like the table of contents or appendix.
