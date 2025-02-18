```toml
name = 'Show'
method = 'GET'
url = '{{server}}/orders/{{orderId}}'
sortWeight = 3000000
id = '25355fb4-cfd8-43c9-8139-d0257ee39e9f'
```

#### Post-response Script

```js
const orderId = jc.response.json("_id")
jc.globals.set("orderId", orderId)

```
