# PolymathDB

An experimental all-in-one database.

## Features
1. Redis API with multithreaded shared-nothing architecture like DragonflyDB.
2. SQL API using go-mysql-server.
3. Custom Bw-Tree storage engine for high-throughput writes and low-latency reads using Pebble as LSM tree storage.
4. Support for both in-memory (like Redis) and on-disk storage using Pebble (like KVRocks).
5. Tiering: https://dicedb.io/docs/features/tiering
6. Subscription, but delivery via a message queue like structure: https://dicedb.io/docs/features/query-subscriptions

## Questions
1. How to do transactions and ACID compliance?
2. How to do message queue and pub/sub?
3. How to do replication and HA?
4. How to integrate Lua scripting engine?

## Related projects
https://github.com/spacejam/sled
https://github.com/dragonflydb/dragonfly
https://github.com/apache/kvrocks
https://github.com/cockroachdb/pebble
https://github.com/dolthub/go-mysql-server
