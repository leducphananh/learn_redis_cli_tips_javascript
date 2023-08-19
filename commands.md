# redis-cli

## Redis string

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

## Redis lists

lpush `key` `element` [element...] -> thêm vào đầu list, nếu không có list thì tạo xong push
lpushx `key` `element` [element...] -> thêm vào đầu list, nếu không có list thì không push
rpush `key` `element` [element...] -> thêm vào cuối list

lrange `key` `start` `stop`

llen `key`

lpop `key` -> lấy phần tử đầu tiên và xóa
rpop `key` -> lấy phần tử cuối cùng và xóa

lset `key` `index` `element` -> set phần tử index bằng element
linsert `key` BEFORE|AFTER `pivot` `element` -> insert before (after) phần tử pivot phần tử element

lindex `key` `index` -> lấy phần tử index

sort `key` (desc) ALPHA -> sắp xếp
