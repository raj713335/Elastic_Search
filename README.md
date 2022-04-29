# Elastic Search

<a href="https://www.youtube.com/watch?v=kjN7mV5POXc&t=3085s">Link</a>

```
GET _search
{
  "query": {
    "match_all": {}
  }
}
```

```GET /_cat/health?v&pretty```

```
PUT /customer/_doc/1?pretty
{
  "name":"John Doe"
}
```

```
PUT /customer/_doc/6
{
  "name":"Elastic Search"
}

POST /customer/_doc/7
{
  "name":"Elastic Search Again"
}
```



```GET /customer/_doc/1```

```console
GET /customer/_search
{
  "query": {"match": {
    "name": "doe"
  }}
}
```


```console
GET /bank/_search
{
  "query":{
    "bool":{
      "must":{
        "match":{
          "address": "Lane street"
        }},
      "filter":{
        "range":{
          "balance":{
            "gte":20000,
            "lte":30000
          }
        }
      }
    }
  }
}
```

