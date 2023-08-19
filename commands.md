# redis-cli

set `key` `value`
get `key`

getrange `key` `start` `end`
strlen `key`

mset `key1` `value1` `key2` `value2` ...
mget `key1` `key2`

del `key1` `key2`

incr `key` -> increase by 1
incrby `key` `number` -> increase by number

decr `key` -> decrease by 1
decrby `key` `number` -> decrease by number

expire `key` `seconds` -> set expire time
ttl `key` -> take time left

keys \* -> get all keys
