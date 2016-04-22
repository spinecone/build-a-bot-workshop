# Personalize your Bot

There are tons of free, easily accessible data sources you can use to create interesting bots. Some of my favorites are:

* 
**Wikimedia** provides free, public APIs for all of their services including Wikipedia and Wikihow. Uses simple GET requests with no authentication required. There is [documentation](https://www.mediawiki.org/wiki/API:Main_page) as well as a [Python wrapper](https://pypi.python.org/pypi/wikipedia/). Cool bots that use the Wikimedia API include [@wikisext](https://twitter.com/wikisext) and [@how2butt](https://twitter.com/how2butt).
* **Tweepy**, the library we used to send tweets from our sample bot, can also be used to search and reply to tweets. Tweepy is very [well documented](http://tweepy.readthedocs.org/en/v3.2.0/).
* **Google** has a lot of different free, public APIs that have basic authentication and usage limit requirements. The whole list of Google APIs is [here](https://developers.google.com/apis-explorer/#p/). [@earthroverbot](https://twitter.com/EarthRoverBot) and [@youareherebot](https://twitter.com/youareherebot/with_replies) use the [Google Maps](https://developers.google.com/maps/?hl=en) API.
* **ITunes** has a [search API](https://www.apple.com/itunes/affiliates/resources/documentation/itunes-store-web-service-search-api.html) that provides information on music, movies, and other media for free and with no authentication.
* **Pokeapi** has a [wealth of pokemon data](http://pokeapi.co/) free and with no authentication steps.


Here's a [mostly complete list of Python API wrappers](https://github.com/realpython/list-of-python-api-wrappers).

It's also possible to make a unique bot without many changes or additions to the template. [@everyportland](https://twitter.com/everyportland) is a bot that has very minor differences from the original template. It tweets from a list of English nouns instead of a book, plus a Portland-specific modifier (i.e. "Natural abacuses").

****
You can check out the source code for these Python Twitter bots for ideas or examples:
*[@tacohelper](http://www.twitter.com/taco_helper) creates fantastical Taco Bell menu items and suggests them to specific people selected by their recent tweets.
* 
[@angryrichpeople](https://github.com/tpinecone/angry_rich_people) posts 1 star reviews of $$$$ Yelp reviews
* 
[@crystalliser](https://github.com/Autophagy/crystalliser-bot) takes an image and "crystallizes" it.
* [@emoji_haiku](https://github.com/williln/emojihaiku) creates haikus out of emoji.
* [@gutendelight](https://github.com/hugovk/gutendelight) makes rhyming couplets out of hip hop lyrics and classic literature.
* 
[@kaikkisanat](https://github.com/hugovk/everyfinnishword) is tweeting every word in Finnish.
* [@permitbot](https://github.com/chagan/permitbot) reports on building permits filed in Chicago.

BotWiki maintains a [list of Twitter bots](https://botwiki.org/bots/twitterbots) which are not all open source or written in Python.



Happy building!

