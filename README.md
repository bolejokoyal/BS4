# BS4
<p>import requests as r <br/>
from bs4 import BeautifulSoup <br/>
response = r.get("[Paste github link here](https://sieskmkb.github.io/ir.github.io/)")<br/>
soup = BeautifulSoup(response.text, 'html.parser')<br/>
print(soup.find("pre", id='keywords').text)
</p>
