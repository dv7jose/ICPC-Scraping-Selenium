# ICPC-Scraping-Selenium

Data Scraper: José Martínez, martinez307jose@gmail.com

For an unreleased investigation coming soon, I scraped all the state official's emails from the ICPC website: http://icpcstatepages.org/ using Selenium.

Given that it's 50 states, I was going to have to figure out how to scrape through all of them in one go. First, I noticed that the url for each state went as follow:
http://icpcstatepages.org/Texas/info/. 

With that in mind, I just created a list of 50 urls and changed just the state name. All that was left was to create a loop that would go through each url in the list and scrape it.

As for the scraping, I first begin by practicing on an individual state, in this case Alabama.

I used Selenium because a lot of the emails were hyperlinks and thus operated under javascript, so BeautifulSoup or any other html parsers wouldn't have gotten the job done.

Then, I had to clean A LOT because some scraped emails included unrelated text, there were duplicates, empty rows, etc.

Finally, everything was exported to nice and simple csv where every email for every state official from every state can be easily accessed.
