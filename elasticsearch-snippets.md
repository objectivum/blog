`GET <host>:<port>/<index-name>/_search?filter_path=took,hits.total,hits.hits._source.*,aggregations.*`
```json
{
  "query": {
    "bool": {
      "should": [
        {
          "bool": {
            "must_not": {
              "nested": {
                "path": "someField",
                "query": {
                  "exists": {
                    "field": "someField"
                  }
                }
              }
            }
          }
        }
      ]
    }
  }
}
```
