# RESTinPy
Ultra-lightweight test suite focused on REST API continuous integration.

## Test a webservice in two lines

It's that simple :

```python
def testPingGoogleHome(self):
  """
  He pings http://google.com
  """
  response = self.get('/')
  return self.expect(response, code=200)
```

Returns :

    [OK] [code : 200] [0:00:00.076603ms]    He pings http://google.com

## One dependency

The only dependency of the RESTinPy project is `requests`.

## Doc

[DIRTY] : means that your code raised an exception. Correct it and try again.
