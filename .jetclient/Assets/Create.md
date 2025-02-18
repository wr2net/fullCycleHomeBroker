```toml
name = 'Create'
method = 'POST'
url = '{{server}}/assets'
sortWeight = 1000000
id = '44a8b4b6-0b4e-4541-898b-10e184072914'

[body]
type = 'JSON'
raw = '''
{
  "name": "Amazon",
  "symbol": "A1",
  "price": 100,
  "image": "AMZN.png"
}'''
```

#### Pre-request Script

```js


```

#### Post-response Script

```js
const assetId = jc.response.json("_id")
const assetSymbol = jc.response.json("symbol")
jc.globals.set("assetId", assetId)
jc.globals.set("assetSymbol", assetSymbol)

```
