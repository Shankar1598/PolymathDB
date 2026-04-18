# PolymathDB

An experimental all-in-one database.

## Features
1. Redis API with multithreaded shared-nothing architecture like DragonflyDB.
2. SQL API using go-mysql-server.
3. Custom Bw-Tree storage engine for high-throughput writes and low-latency reads using Pebble as LSM tree storage.
4. Support for both in-memory (like Redis) and on-disk storage using Pebble (like KVRocks).

## Questions
1. How to do transactions and ACID compliance?
2. How to do message queue and pub/sub?
3. How to do replication and HA?
4. How to integrate Lua scripting engine?
