# url-short-cutter-API


The package implements simple microservice with REST interface taking an URL and returning a short URL, which is stored in mongoDB.

## Examples

In order to use it, pass the url variable to the POST or GET request at http://localhost:8081/v1, for example, like this:

```sh
curl http://localhost:8081/v1?url=https://golang.org/doc/
```

The latter in python: 

```python
>>> import requests
>>> r = requests.get('http://localhost:8081/v1', params={'url': 'https://golang.org/doc/'})
>>> print(r.text)
localhost:8081/m62Kc
>>> 
```
