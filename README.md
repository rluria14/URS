# Reddit Scraper for Penetration Testing posts

You will need to install the PRAW module in order for this program to work. `pip install praw` or `pip3 install praw` depending on your system. You will also need your own Reddit account and API credentials.

**NOTE:** PRAW currently only supports Python 2.7, 3.3, 3.4, 3.5, and 3.6.

This is a Reddit scraper I created using the Reddit API. It is designed specifically to scrape for penetration testing information within the following subreddits:
 - Pentesting
 - AskNetSec
 - HowToHack
 - netsec
 - hacking
 - netsecstudents
 - raspberry_pi
 - homelab
 - Kalilinux
 - Hacking_Tutorials
 - pentest

You can choose which category of posts to scrape each subreddit as well as how many results are returned. These options include:
 - Hot
 - New
 - Controversial
 - Top
 - Rising
 - Search - Users also have the option to search each subreddit for keywords; however, all search results are returned and the number of results the user specifically wants is disregarded.

# How to get Reddit API Credentials

First, create your own Reddit account and then head over to https://old.reddit.com/prefs/apps.

Click "create app". Name your app and choose "script" for the type of app. In the redirect URL, type in "http://localhost:8080" since this is a personal use app. You can also add a description and an about URL. 

Once you create the app, you should see a string of 14 characters on the top left corner underneath "personal use script." That is your API ID. Further down you will see "secret" and a string of 27 characters; that is your API password. You'll need to save this information as it will be used in the program in order to use the Reddit API. You'll also have to provide your app name, Reddit account username and password as well. 

This block of credentials is found on lines 14-18.

# How to modify this program to scrape other subreddits

This program can be easily modified to scrape any subreddit(s). All you have to do is change the list of subreddits to scrape on line 21 to the subreddits you want. Also change the text in the subreddit selection loop as to avoid confusion.

Enjoy!
