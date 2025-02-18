```toml
name = 'Create Asset'
method = 'POST'
url = '{{server}}/wallets/{{walletId}}/assets'
sortWeight = 4000000
id = '13e0c0fd-67a9-41a9-8554-9309e3cbf7e8'

[body]
type = 'JSON'
raw = '''
{
  "assetId": "{{assetId}}",
  "share": 100
}'''
```
