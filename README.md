# Python-Cheatcode

### JSON to Pandas dataframe

```python
import json 
import requests
import pandas as pd
url = 'https://newsapi.org/v2/top-headlines?country=us&apiKey=7da74b8009ae4c098a9c5d8942f48417'
request  = requests.get(url).json()
title = request['articles'][0]['title']
print (title)
```
