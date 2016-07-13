
# Set up a GitHub account
<img src="Screen Shot 2016-07-12 at 10.58.03 PM.png" height="350"><br>
The template we're going to base a new bot on, Hello World Bot, is made up of 6 files.
* **README.md** is a file that most GitHub repos have. It describes what the project does and how to use it.
* **book.txt** is where the text of a book will go.
* **book_manager.py** handles the logic of getting lines out of our book file, and deleting them after they're tweeted.
*  **bot.py** handles authenticating with Twitter and posting tweets. Finally, **secrets.py** will hold our authentication secrets which we'll cover in the next section. **secrets.py** is not included in the template repo since we don't want to make our authentication info publicly accessible.

* 
If you don't have a GitHub account, you'll need to create one first at https://github.com/join (the free version will be fine)

##What did we just do?
GitHub is a service that allows us to share projects with others. It uses Git, a program for keeping track of changes to a project. There's nothing about Git or GitHub that's specific to programming. You could use it to keep track of changes to a novel or any other project you might want to share with other people, as long as it can be represented as a group of files. For this tutorial, we're going to be taking "hello-world-bot," an example Twitter bot that's hosted on GitHub, copying it, and turning it into a whole new bot.

Git and GitHub are very complex and have a lot of different features that we won't be covering in this tutorial. If you're interested in getting started with Git and GitHub, I highly recommend the <a href="https://dont-be-afraid-to-commit.readthedocs.io/en/latest/">Don't Be Afraid to Commit</a> tutorial.


