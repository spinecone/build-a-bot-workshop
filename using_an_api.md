# Using an API
An API is a set of instructions that programs can use to talk to each other. In web development, these instructions are usually defined as a set of urls that can take different parameters.

To make a Twitter bot, you might use an API to collect boring data and do something interesting to it. For example, <a href="https://twitter.com/how2butt">@how2butt</a> uses the url ```http://www.wikihow.com/api.php?action=query&list=random&rnnamespace=0&rnlimit=1&format=json``` from the <a href="https://www.mediawiki.org/wiki/API:Main_page">MediaWiki API</a> to find a random WikiHow article. Then, in order to make the world a better place, it replaces one of the words in the article's title with "butt."

Let's use a simpler example to look at how an API works. Try visiting the url ```http://pokeapi.co/api/v2/pokemon/1/``` in your browser.

This url is an endpoint of the Pokéapi. It has extensive documentation at https://pokeapi.co/ which describes all the different kinds of urls you can use to see Pokemon data.

The pile of text you're seeing is JSON, a data format that most programming languages can understand.

<center><img height="100" src="001Bulbasaur_Dream.png"><br>"I'm machine-readable!"
</center>

We can use Python's <a href="http://docs.python-requests.org/en/master/">requests</a> and <a href="http://docs.python-guide.org/en/latest/scenarios/json/">json</a> libraries to read from JSON urls like this one:
<img src="Screen Shot 2016-07-13 at 9.09.59 PM.png">

Now all you have to do is pass the text you've created to Tweepy. You can read data from pretty much an API just using requests.get() and json()!



