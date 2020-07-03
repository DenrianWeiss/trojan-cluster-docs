Trojan-cluster Deploy Maunal
===

## Get Binary

Navigate to the Azure Pipeline and download the latest binary.

## How to configure

Basically, the trojan-redis branch shares the same configure process of the original trojan, however you need to enable trojan by adding this to the configure file:
```JSON
redis: {
    "enabled": true,
    "server_addr": your_redis_server_here,
    "server_port": your_redis_port
}
```

The server info is optional, as if not exists, it will be set to the default value of `127.0.0.1` `6379`.
