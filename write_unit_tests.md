# Write unit tests for your bot

Sweet! Your bot is tweeting on a schedule, and you're on your way to Twitter bot superstardom! But what if you want to add some changes to your bot down the line? How can we verify that your changes won't break any of the current behavior?

We can safely make changes and additions to our bot through the magic of ✨unit tests✨!

Unit tests check that every small part of a program works the way a programmer expects it to. For example, if you were programming a vending machine, you might write a unit test that checks that the machine gives you chips that cost a dollar if you put a dollar into the machine, but won't give you the chips if you only put in 50 cents. 

There are 3 unit tests that are included in the hello-world-bot template. The tests check that:
1. The bot will tweet sentences that are less than 140 characters.
* If a sentence is longer than 140 characters, the bot will tweet up to 140 characters of it.
* After tweeting, the bot will remove the text it just tweeted from the book file.

You can run the tests with ```python3 tests.py```. However, depending on the changes you made to personalize your bot, these tests probably aren't valid anymore. Let's go over how these basic tests work, and you can change them to fit your bot.

