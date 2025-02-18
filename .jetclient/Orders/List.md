```toml
name = 'List'
method = 'GET'
url = '{{server}}/orders/{{walletId}}'
sortWeight = 2000000
id = 'a2e20666-dbb3-489f-8175-58e95a353e0f'
```

#### Post-response Script

```js
const orderId = jc.response.json("_id")
jc.globals.set("orderId", orderId)

```
