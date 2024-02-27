# Fashion AI API
by [Tony Assi](https://www.tonyassi.com/)

Email me for a free API key <tony.assi.media@gmail.com>

## Basic Usage
Calling the image segmentation endpoint in Python:
```python
import requests

url = 'https://tonyassi-fashion-api.hf.space/segment_clothing'
myobj = {
    "key": "YOUR_KEY",
    "url": "https://media.lucyinthesky.com/data/Feb24/850xAUTO/4a6b2989-9342-45b0-8566-10060d05d9f2.jpg"
    }

response = requests.post(url,  json = myobj)
print(response.text)
```
