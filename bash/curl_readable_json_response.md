# Curling and readable json-response
I often use `curl` to take a quick look at the responses of particular endpoints. And often the response is in JSON-formatted I wanna see in **readable** format instead of a floating text:

```bash
curl ... | json_pp 
```

Or with `jq` using a identity filter…
```bash
curl ... | jq '.'
```
