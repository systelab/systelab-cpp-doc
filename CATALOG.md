# `systelab-cpp-doc` — A catalog of CSW shared libraries for C++

There are a number of libraries that are shared among the different C++ projects that are developed at Werfen Clinical Software. This document is intended to offer a catalog where these libraries and their respective repositories are gathered.

Each library is listed together with a description, the repository where it can be found and other related components that may be of use (if any).


## Catalog
* [cpp-patterns](#cpp-patterns)
* [cpp-webserver-adapter](#cpp-webserver-adapter)
* [cpp-encryption-adapter](#cpp-encryption-adapter)
* [cpp-db-adapter](#cpp-db-adapter)
* [cpp-gtest-allure-utilities](#cpp-gtest-allure-utilities)
* [cpp-hash-utils](#cpp-hash-utils)
* [cpp-json-adapter](#cpp-json-adapter)
* [cpp-json-settings](#cpp-json-settings)
* [cpp-jwt-utils](#cpp-jwt-utils)
* [cpp-rest-api-core](#cpp-rest-api-core)
* [cpp-test-utilities](#cpp-test-utilities)
* [cpp-time-adapter](#cpp-time-adapter)
* [cpp-trace-api](#cpp-trace-api)
* [cpp-websockets-adapter](#cpp-websockets-adapter)

### cpp-patterns <a name="cpp-patterns"></a>
Collection of C++ implementation for design patterns.
##### Repository
https://github.com/systelab/cpp-patterns


### cpp-webserver-adapter <a name="cpp-webserver-adapter"></a>
A library-agnostic API for C++ to work with a web server. Supported features include:
* Server and client
* HTTP
* HTTPS
* Mutual SSL
* CORS
* Thread pool
* GZIP compression
##### Repository
https://github.com/systelab/cpp-patterns
##### Related components
* [cpp-boostasio-webserver-adapter](https://github.com/systelab/cpp-boostasio-webserver-adapter)
* [cpp-httplib-webserver-adapter](https://github.com/systelab/cpp-httplib-webserver-adapter)

### cpp-encryption-adapter <a name="cpp-encryption-adapter"></a>
A library-agnostic API for C++ to encrypt data.
##### Repository
https://github.com/systelab/cpp-encryption-adapter
##### Related components
* [cpp-caeser-cypher-encryption-adapter](https://github.com/systelab/cpp-caeser-cypher-encryption-adapter)

### cpp-db-adapter <a name="cpp-db-adapter"></a>
A library-agnostic API for C++ to work with a database. Supported features include:
* Table queries
* Table record insert, update and delete
* SQL queries
* Transactions
##### Repository
https://github.com/systelab/cpp-db-adapter
##### Related components
* [cpp-sqlite-db-adapter](https://github.com/systelab/cpp-sqlite-db-adapter)

### cpp-gtest-allure-utilities <a name="cpp-gtest-allure-utilities"></a>
Utilities to generate Allure reports for automated tests based on GoogleTest.
##### Repository
https://github.com/systelab/cpp-gtest-allure-utilities

### cpp-hash-utils <a name="cpp-hash-utils"></a>
Utilities to generate Allure reports for automated tests based on GoogleTest.
##### Repository
https://github.com/systelab/cpp-hash-utils

### cpp-json-adapter <a name="cpp-json-adapter"></a>
A library-agnostic API for C++ to work with JSON documents. Supported features include:
* JSON parsing
* String serialization
* JSON pointers
* JSON schema validation
* Unicode
##### Repository
https://github.com/systelab/cpp-json-adapter
##### Related components
* [cpp-rapidjson-json-adapter](https://github.com/systelab/cpp-rapidjson-json-adapter)

### cpp-json-settings <a name="cpp-json-settings"></a>
Utilities to save/load configuration settings on JSON files. Supported features include:
* Compile-time error detection
* Basic types: string, boolean, integer and double
* Sections hierarchy
* In-memory cache
* Encryption of JSON files
##### Repository
https://github.com/systelab/cpp-json-settings

### cpp-jwt-utils <a name="cpp-jwt-utils"></a>
Utilities to generate, parse and validate JWTs (JSON Web Tokens) used to implement an authentication mechanism over a REST API.
##### Repository
https://github.com/systelab/cpp-jwt-utils

### cpp-rest-api-core <a name="cpp-rest-api-core"></a>
Implementation of a C++ framework to facilitate the creation of REST API. Supported features include:
* Routing mechanism
* Authorization through JWT
* User access validation
* Token expiration validation
* Custom access validation
##### Repository
https://github.com/systelab/cpp-rest-api-core

### cpp-test-utilities <a name="cpp-test-utilities"></a>
Common interface for the test utilities used by the different C++ projects of Systelab organization.
##### Repository
https://github.com/systelab/cpp-test-utilities

### cpp-time-adapter <a name="cpp-time-adapter"></a>
Utilities to access system time.
##### Repository
https://github.com/systelab/cpp-time-adapter

### cpp-trace-api <a name="cpp-trace-api"></a>
Utilities to easily add traces to your application. Supported features include:
* Multiple channels
* Dump to .log files
* Dedicated threads
* Built-in fields
* Channel enabling/disabling
* Severity filtering
* Backup generation
* Deletion of old backups (rolling basis)
##### Repository
https://github.com/systelab/cpp-trace-api

### cpp-websockets-adapter <a name="cpp-websockets-adapter"></a>
A library-agnostic API for C++ to work with a web sockets. Supported features include:
* Server and client
* WSS
* Send messages to server
* Push notifications to all clients
##### Repository
https://github.com/systelab/cpp-websockets-adapter
##### Related components
* [cpp-websocketpp-adapter](https://github.com/systelab/cpp-websocketpp-adapter)
