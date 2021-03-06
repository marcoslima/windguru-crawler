# Simple WindGuru Crawler

Simple web-crawler using BeautifulSoup and webdriver to get precipitation data from [windguru](https://www.windguru.com/263).

This is just a POC - should not to be used in production.

  - You can change it to your city...
  - You can change to get more data...
  - You can change to whatever you need/want...

### Installation

You need to have nodejs and python3 (and npm and pip3).
You also need [phantomjs](http://phantomjs.org/download.html) or [chromedriver](https://sites.google.com/a/chromium.org/chromedriver/downloads)

Install the dependencies...

```sh
$ cd windguru-crawler
$ pip install -r requirements.txt
```

To run...

```sh
$ python3 rain.py
```

expected output...
```sh
Starting windGuru crawler...
trying number 1
09h: -
12h:  
15h:  
18h: 0.3
21h: 1.5
DONE
```
Where **0.3** is the precipitation in milimeters. Any doubts on the data, come [here](https://www.windguru.cz/help.php?sec=intro) and search for **Precipitation**

PS. If doesn't work, try to increase the SLEEP_FOR var... also, hit the URL on the browser and try above on the console:

```sh
document.getElementById('div_wgfcst0')
should output
<div class="obal-wrap" id="div_wgfcst0"></div>
```

License
----
GNU Affero General Public License v3.0

