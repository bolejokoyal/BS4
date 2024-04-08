# BS4
<p>import requests as r <br/>
from bs4 import BeautifulSoup <br/>
response = r.get("https://bolejokoyal.github.io/cc.github.io/")<br/>
soup = BeautifulSoup(response.text, 'html.parser')<br/>
print(soup.find("pre", id='keywords').text)
</p>

<pre>import requests

url = "https://open-ai21.p.rapidapi.com/conversationgpt35"

payload = {
	"messages": [
		{
			"role": "user",
			"content": "Sum of N numbers in python"
		}
	],
	"web_access": False,
	"system_prompt": "",
	"temperature": 0.9,
	"top_k": 5,
	"top_p": 0.9,
	"max_tokens": 256
}
headers = {
	"content-type": "application/json",
	"X-RapidAPI-Key": "c4e2808293msh16778298359d982p185654jsn8c828c507815",
	"X-RapidAPI-Host": "open-ai21.p.rapidapi.com"
}

response = requests.post(url, json=payload, headers=headers)

print(response.json())</pre>
