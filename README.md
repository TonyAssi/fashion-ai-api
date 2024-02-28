# Fashion AI API
by [Tony Assi](https://www.tonyassi.com/)

Email me for a free API key <tony.assi.media@gmail.com>

## Basic Usage
Calling the image segmentation endpoint in Python:
```python
import requests

url = 'https://tonyassi-fashion-api.hf.space/segment_clothing'
data = {
    "key": "YOUR_KEY",
    "url": "https://assets.vogue.com/photos/63c9504e426d4c71724c337b/master/w_1280%2Cc_limit/00001-rains-fall-2023-menswear-credit-filippo-fior-brand.jpg"
    }

response = requests.post(url,  json=data)
print(response.text)
```
## API
### Get Credits
get the number of remaining credits left in your account
```python
import requests

url = 'https://tonyassi-fashion-api.hf.space/get_credits'
data = {
    "key": "YOUR_KEY"
    }

response = requests.post(url,  json=data)
print(response.text)
```
### Segment Clothing
accepts an image url, returns a .png of the segmented clothing
```python
import requests

url = 'https://tonyassi-fashion-api.hf.space/segment_clothing'
data = {
    "key": "YOUR_KEY",
    "url": "https://assets.vogue.com/photos/63c9504e426d4c71724c337b/master/w_1280%2Cc_limit/00001-rains-fall-2023-menswear-credit-filippo-fior-brand.jpg"
    }

response = requests.post(url,  json=data)
print(response.text)
```
![display1](https://github.com/TonyAssi/fashion-ai-api/assets/42156881/a07b59f0-02ab-492d-8e89-52fe2bf22d1e)

### Image to Fashion Article
accepts an image url, returns a fashion article in the style of Vogue magazine
```python
import requests

url = 'https://tonyassi-fashion-api.hf.space/fashion_article'
data = {
    "key": "YOUR_KEY",
    "url": "https://assets.vogue.com/photos/63c9504e426d4c71724c337b/master/w_1280%2Cc_limit/00001-rains-fall-2023-menswear-credit-filippo-fior-brand.jpg"
    }

response = requests.post(url,  json=data)
print(response.text)
```
