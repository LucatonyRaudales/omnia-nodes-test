curl -X POST --data '{
    "jsonrpc":"2.0",
    "id"     :1,
    "method" :"info.isBootstrapped",
    "params": {
        "chain":"C"
    }
}' -H 'content-type:application/json;' 127.0.0.1:9650/ext/info


https://docs.avax.network/community/tutorials-contest/2021/red-dev-avalanche-chainlink-tutorial