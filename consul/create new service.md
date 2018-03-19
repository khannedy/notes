## Service Definition

```json
{
  "ID": "elasticsearch-9200",
  "Name": "elasticsearch",
  "Tags": [],
  "Address": "127.0.0.1",
  "Port": 9200,
  "Check": {
    "Interval": "10s",
    "HTTP": "http://127.0.0.1:9200/"
  }
}
```

## Register to Consul

```bash
curl -XPUT --data @consul.json "http://localhost:8500/v1/agent/service/register"
```

## Deregister from Consul

```bash
curl -XPUT "http://localhost:8500/v1/agent/service/deregister/my-service-id"
```
