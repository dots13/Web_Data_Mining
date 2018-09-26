# 1. Data Acquisition - Web Crawler/Scraper
## Task
* Select a web source of your own choice for the non-trivial web crawling task.
** The resource should contain hundreds/thousands of unique pages to crawl.
** Each page should contain at least:
*** Title - e.g. an article title, a product title, …
*** Main content/text - a main text of the article, a description of the product, …
*** Additional features describing the page - information about author, date of publishing, product item parameters, …
* Identify possible issues with crawling:
** Explore the robot exclusion protocol, availability of the sitemaps description, …
** Identify issues with extraction of relevant information
*** Extraction using machine readable annotations, own set of rules/selectors, automatic detection of the content, …
* Properly design and implement the extraction task
** Inputs and outputs of the task
** Dealing with policies
** Selection of the language/tools
* Configure the crawler
** focus on crawling of just one single host (domain)
**  set the crawl interval! Otherwise you can be banned!
** set the crawl depth
** user-agent string
** seed URLs
** and other settings you consider important.