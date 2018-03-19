## Server Configuration

```json
{
  "bootstrap" : true,
  "server" : true,
  "datacenter" : "wallet",
  "data_dir" : "data",
  "log_level" : "INFO",
  "bind_addr" : "127.0.0.1",
  "client_addr" : "127.0.0.1"
}
```

## Client Configuration

```json
{
	"server" : false,
	"datacenter" : "DEV1-CLUSTER",
	"data_dir" : "/opt/var/consul",
	"log_level" : "INFO",
	"bind_addr" : "192.168.0.5",
	"client_addr" : "192.168.0.5",
	"start_join" : [
		"192.168.0.1",
		"192.168.0.2",
		"192.168.0.3"
	]
}
```

## Start Agent

```bash
./consul agent -ui -config-dir ./config
```
