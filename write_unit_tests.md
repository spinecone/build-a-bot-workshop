# Write unit tests for your bot

Sweet! Your bot is tweeting on a schedule, and you're on your way to Twitter bot superstardom! But what if you want to add some changes to your bot down the line? How can we verify that your changes won't break any of the current behavior?

We can safely make changes and additions to our bot through the magic of ✨unit tests✨!

Unit tests check that every small part of a program works the way a programmer expects it to. For example, if you were programming a vending machine, you might write a unit test that checks that the machine gives you chips if you put a dollar into the machine, and another test that it won't give you the chips if you only put in 50 cents. 

In general, every unit test consists of some setup and one or more assertions. Here's how that might look with the vending machine from earlier.

<img src="Screen Shot 2016-07-13 at 12.12.43 AM.png">

The setup for both of these tests is that we initialize a VendingMachine object, and put some money into it. In the first test, we assert that "chips" is what we get back after inserting 1 money, essentially a dollar. The second test asserts is that "NOT ENOUGH!" is what the machine returns for .5 money. We would prefer to receive proper edible chips from a real machine, but for the purposes of unit testing, the string "chips" will be just fine.

Once these tests are in place, we can update the vending machine to accept different amounts of money and return different kinds of items knowing that we won't break our dollar chips behavior without realizing it.

There are 3 unit tests that are included in the hello-world-bot template. The tests check that:
1. The bot will tweet sentences that are less than 140 characters.
* If a sentence is longer than 140 characters, the bot will tweet up to 140 characters of it.
* After tweeting, the bot will remove the text it just tweeted from the book file.

You can run the tests with ```python3 tests.py```. However, depending on the changes you made to personalize your bot, these tests probably aren't valid anymore. Let's go over how these basic tests work(ed), and you can change them to fit your bot.

<img src="Screen Shot 2016-07-12 at 11.46.02 PM.png">
Since we don't want to affect the book we're actually tweeting from, we use a temporary file ("test_file") that we create and destroy in each test. For this test, the test_file just has two short sentences, in order to assert that get_next_chunk() will return the entire first sentence if it's short enough.

