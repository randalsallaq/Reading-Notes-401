# Web Scrabing:

#### "Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites. Web scraping software may access the World Wide Web directly using the Hypertext Transfer Protocol, or through a web browser. While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying, in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis."

![d](https://www.octoparse.com/media/7529/web-scraping-introduction.jpg?width=666&height=480)


### Import ..

`import requests`

`import urllib.request`

`import time`

`from bs4 import BeautifulSoup`


### use URL library

`url = 'http://web.mta.info/developers/turnstile.html'`

`response = requests.get(url)`


### Parse it with BeautifulSoap

`soup = BeautifulSoup(response.text, “html.parser”)`

`soup.findAll('a')`


### extract

`one_a_tag = soup.findAll(‘a’)[38]`

`link = one_a_tag[‘href’]`


`download_url = 'http://web.mta.info/developers/'+ link`

`urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:])`


`time.sleep(1)`
