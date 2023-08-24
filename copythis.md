from bs4 import BeautifulSoup as bs
import requests as re

url = 'https://www.semrush.com/blog/most-visited-websites/'

response = re.get(url)

if response.status_code == 200:
    print("Request successful.")
else:
   print("Not successful your code was " + str(response.status_code))

found_links = soup.find_all('title')
print(found_links)
