# Elastic_Search

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

```
console
GET /customer/_search
{
  "query": {"match": {
    "name": "doe"
  }}
}
```

