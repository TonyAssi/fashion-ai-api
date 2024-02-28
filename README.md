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
![00001-rains-fall-2023-menswear-credit-filippo-fior-brand](https://github.com/TonyAssi/fashion-ai-api/assets/42156881/b12fd12c-1d5c-43d9-ae40-17d78501892e)


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
![VO100118_western07 copy](https://github.com/TonyAssi/fashion-ai-api/assets/42156881/7cb8ab48-3979-41c3-9297-6b860abc4ee4) 
Step into a world of whimsical fashion with this captivating ensemble from Versace, as showcased in a recent official editorial featuring Lalisa Manobal, more famously known as \"Lalisa\" of Blackpink. Taking inspiration from the boho chic style, this colorful dress teases with a cluster of vibrant reds, whites, and blacks that evoke the irresistible charm of a picturesque summer festival. Effortlessly veering from a traditional, streamlined look, the dress naturally catches the eye with its bold patterns and infectious energy. Lalisa's presence in this promotional shot for Harpers Bazaar only serves to amp up excitement for the trendsetting fashion of 2020.\n\n*\n\nThe dress is not the only piece that commands attention; the patterned scarf, too, adds a beautiful touch to the ensemble. Draped around the shoulders, this vibrant accessory exhibits a variety of reds, whites, and blacks that complement the dress perfectly. Here, Lalisa seems to defy gravity itself, standing tall on stilts and posing gracefully for the camera. Is it the dress? The scarf? The stilts that lend her supermodel poise? It's difficult to say, but one thing is certain - she's fully embracing the bohemian spirit of this outfit.\n\n\n\nThe third element that steals the show is Anya Taylor-Joy. In case her name didn't ring a bell, Anya is a beloved model who's no stranger to captivating the public's eye with her eclectic style. Wearing this same outfit, she effortlessly showcases how anyone can adopt the boho chic vibe. Her appearance on Model Society proves that this trend isn't reserved for festival-goers or free-spirited souls - it's for anyone who loves to dance on the fashion dividing line, defying expectations with daring yet elegant choices. Long live the boho chic spirit!\n\n\n\nThe combination of the colorful dress, patterned scarf, and the presence of two such fabulous women brings the vibrant energy of a carefree summer party to life. The setting, too, reflects the unapologetic flair of the bohemian mindset. As you gaze into the heart of the shot, you can't help but wonder what adventures could unfold just by following this stylish lead, basking in the glow of the lively decor and enchanting performers around you.\n\n\n\nAs we look beyond the image itself, we find more proof that the boho chic thrill doesn't stop at the outfit. This escape from the ordinary is a lifestyle choice. The freedom to express one's true self without restraint is intoxicating, and it's clear that Lalisa, Anya, and the rest of the fashion world have embraced the opportunity. From the uplifting colors and patterns to the hair, makeup, and accessories, this ensemble is the ultimate embodiment of the charming yet rebellious spirit of boho chic. Go ahead - let your hair down and embrace the magic of the 2020 fashion world.
