# meta parser

meta parser is parser of HTML meta tag for Python.


## How to use it?

```
>>> from metaparser import HTMLMetaParser
>>> from urllib import request
>>> parser = HTMLMetaParser()
>>> resp = request.urlopen('https://github.com/')
>>> parser.feed(str(resp.read()))
>>> parser.og_image_url
'https://assets-cdn.github.com/images/modules/open_graph/github-octocat.png'
>>> parser.og_description
'GitHub is the best place to build software together. Over 4 million people use GitHub to share code.'
```


## License

MIT
