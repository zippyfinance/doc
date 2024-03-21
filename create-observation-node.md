---
description: This chapter will introduce how to create observation nodes to everyone.
---

# Create observation node

1. Download the zippynode binary file from the link http://64.71.185.50/download/zippynode.

```
http://64.71.185.50/download/zippynode
```

{% code title="observation/explorer node command" overflow="wrap" lineNumbers="true" %}
```
./zippynode --log_folder ./tmp_log --min_peers 4 --bootnodes /ip4/64.71.185.50/tcp/19876/p2p/QmfWjyu4V5SLMYbNCmLu38Lw1eQ4KgsXigyupoWdL36dSv --network_type=localnet --verbosity=5 --p2p.security.max-conn-per-ip=200 --ip 0.0.0.0 --port 19002 --sync --sync.stagedsync --db_dir ./testdb/ --broadcast_invalid_tx=false --http.ip=0.0.0.0 --ws.ip=0.0.0.0 --run=explorer --run.shard=0
```
{% endcode %}

1. \--log\_folder ./tmp\_log is used to set the log file.
2. \--min\_peers 4 is used to set peer numbers.
3. Our bootnode is /ip4/64.71.185.50/tcp/19876/p2p/QmfWjyu4V5SLMYbNCmLu38Lw1eQ4KgsXigyupoWdL36dSv
4. network\_type=localnet is used to set as localnet
5. \--run.shard=0 is used to connect to the shard0, --run.shard=1, --run.shard=2, --run.shard=3 for other shards.
