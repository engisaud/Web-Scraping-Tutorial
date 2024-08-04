# Web-Scraping-Tutorial
import requests
from bs4 import BeautifulSoup
import csv
import pandas as pd
import requests


url = 'https://scrapeme.live/shop/'
response = requests.get(url)
import requests

x = requests.get('https://scrapeme.live/shop/')
print(x.status_code)


import requests
from bs4 import BeautifulSoup

url = 'https://scrapeme.live/shop/';
r = requests.get(url)



soup = BeautifulSoup(r.content, 'html5lib') 
print(soup.prettify())



movies = []
df.to_csv('top-rated-movies.csv', index=False)


import csv

with open('thefile.csv', 'rb') as f:
  data = list(csv.reader(f))

import collections
counter = collections.defaultdict(int)
for row in data:
    counter[row[0]] += 1


writer = csv.writer(open("/path/to/my/csv/file", 'w'))
for row in data:
    if counter[row[0]] >= 4:
        writer.writerow(row)


        infile = "./log_file.log"
with open(infile) as f:
    lines = f.readlines()

df = pd.DataFrame(columns=["time", "type", "value", "unit", "id", "name"])
