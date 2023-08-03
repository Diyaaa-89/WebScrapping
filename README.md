# WebScrapping

import requests
from bs4 import BeautifulSoup

req = requests.get("https://scholarships.gov.in/")

soup = BeautifulSoup(req.content, "html.parser")

print(soup.prettify())
