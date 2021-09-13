# Intro-to-polite-Web-Scraping-of-Soccer-Data-with-R

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.

Fans of soccer/football have been left bereft of their prime form of entertainment these past few months and I’ve seen a huge uptick in the amount of casual fans and bloggers turning to learning programming languages such as R or Python to augment their analytical toolkits. Free and easily accessible data can be hard to find if you only just started down this path and even when you do, you’ll find that eventually dragging your mouse around and copying stuff into Excel just isn’t time efficient or possible. The solution to this is web scraping! However, I feel like a lot of people aren’t aware of the ethical conundrums surrounding web scraping (especially if you’re coming from outside of a data science/programming/etc. background …and even if you are I might add). I am by no means an expert but since I started learning about all it I’ve tried to “web scrape responsibly” and this tenet will be
emphasized throughout this blog post.

Web Scraping Responsibly
========================

When we think about R and web scraping, we normally just think straight to loading {rvest} and going right on our merry way. However, there are quite a lot of things you should know about web scraping practices before you start diving in. “Just because you can, doesn’t mean you should.” robots.txt is a file in websites that describe the permissions/access privileges for any bots and crawlers that come across the site. Certain parts of the website may not be accessible for certain bots (say Twitter or Google), some may not be available at all, and in the most extreme case, web scraping may even be prohibited. However, do note that just because there is no robots.txt file or that it is permissive of web scraping does not automatically mean you are allowed to scrape. You should always check the website’s “Terms of Use” or similar pages.

Web scraping takes up bandwidth for a host, especially if it houses lots of data. So writing web scraping bots and functions that are polite and respectful of the hosting site is necessary so that we don’t inconvenience websites that are doing us a service by making the data available for us for free! There’s a lot of things we take for granted, especially regarding free soccer data, so let’s make sure we can keep it that way.

This blog post will mainly focus on using {rvest} in combination with the {polite} package.

Soccer Data 
=============
1. https://www.transfermarkt.com/
2. https://int.soccerway.com/
3. https://en.wikipedia.org/wiki/Main_Page
