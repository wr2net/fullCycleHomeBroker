```toml
name = 'Create'
method = 'POST'
url = '{{server}}/orders'
sortWeight = 1000000
id = '6a3fe563-0053-447d-8975-f89fae63c717'

[body]
type = 'JSON'
raw = '''
{
  "walletId": "{{walletId}}",
  "assetId": "{{assetId}}",
  "shares": 10,
  "price": 100,
  "type": "BUY"
}'''
```

#### Post-response Script

```js
const orderId = jc.response.json("_id")
jc.globals.set("orderId", orderId)

```
