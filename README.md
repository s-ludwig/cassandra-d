cassandra-d
===========

D language cassandra client (currently binary API v1 and v2).

Currently this driver can be used to create / insert / update / delete data in a cassandra datastore.

There are currently no helpers, you can only execute CQL inputting or retrieving data.

[![Build Status](https://travis-ci.org/s-ludwig/cassandra-d.svg?branch=master)](https://travis-ci.org/s-ludwig/cassandra-d)

## Fork note

This fork adds support for DUB and cleans up the source code and API.

## Working
- Version 1 of the protocol
- Queries
- Prepared Statements

## TODO
- Support version 3/4 of the protocol
- UUID stuff
- Authenticators
- Provide helper functions/templates

## Building the test

- cd source/cassandra
- dmd -main -unittest cql.d serialize.d utils.d tcpconnection.d
OR
- dmd -main -unittest cql.d serialize.d utils.d tcpconnection.d -version=CassandraV2
