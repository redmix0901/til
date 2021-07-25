``` php
acme.sh --issue -d ams.topdev.asia --dns \
 --yes-I-know-dns-manual-mode-enough-go-ahead-please
```

```php
Output => 
Add the following TXT record:
Domain: '_acme-challenge.ams.topdev.asia'
TXT value: 'fZeXjFIZXxAIR5A1B-siwJQP5EEG6u--_3AJr3jSdjo'
```

Thêm record TXT vào DNS với 2 giá trị output trên

```javascript
acme.sh --renew -d ams.topdev.asia \
  --yes-I-know-dns-manual-mode-enough-go-ahead-please
```

Reload lại nginx

```javascript
nginx -s reload
```