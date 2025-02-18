```toml
name = 'Create'
method = 'POST'
url = '{{server}}/wallets'
sortWeight = 1000000
id = '9346f74d-f7fa-4c14-a579-801ceb44a86b'
```

#### Post-response Script

```js
const walletId = jc.response.json("_id")
jc.globals.set("walletId", walletId)

```
