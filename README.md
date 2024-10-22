this works:

```
echo -n '{ "version": "1.1", "host": "example.org", "short_message": "A short message", "level": 5, "_some_info": "foo"}' | nc -u 127.0.0.1 12201
```

and this fails:
```
echo -n '{ "version": "1.1", "host": "example.org", "short_message": "A short message", "level": 5, "_some_info": "foo", "timestamp": 1385053862.3072}' | nc -u 127.0.0.1 12201 
```
