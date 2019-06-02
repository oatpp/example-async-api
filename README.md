# Async API Example [![Build Status](https://dev.azure.com/lganzzzo/lganzzzo/_apis/build/status/oatpp.example-async-api?branchName=master)](https://dev.azure.com/lganzzzo/lganzzzo/_build?definitionId=16&branchName=master)

Example project how-to use oat++ (AKA oatpp) asynchronous API.

See more:

- [Oat++ Website](https://oatpp.io/)
- [Oat++ Github Repository](https://github.com/oatpp/oatpp)
- [Get Started](https://oatpp.io/docs/start)

## Overview

### Project layout

```
|- CMakeLists.txt                        // projects CMakeLists.txt
|- src/
|    |
|    |- controller/                      // Folder containing controller where all endpoints are declared
|    |- dto/                             // DTOs are declared here
|    |- AppComponent.hpp                 // Service config
|    |- App.cpp                          // main() is here
|
|- test/                                 // test folder
|- utility/install-oatpp-modules.sh      // utility script to install required oatpp-modules.
```

---

### Build and Run

#### Using CMake

**Requires**

- `oatpp` module installed. You may run `utility/install-oatpp-modules.sh` 
script to install required oatpp modules.

```
$ mkdir build && cd build
$ cmake ..
$ make 
$ ./example-async-api-exe  # - run application.

```

#### In Docker

```
$ docker build -t example-async-api .
$ docker run -p 8000:8000 -t example-async-api
```

## Read More

- [Simple API vs Async API](https://oatpp.io/docs/simple-vs-async/)
- [Async](https://oatpp.io/docs/async/)
- [Oatpp-Coroutines](https://oatpp.io/docs/oatpp-coroutines/)
- [ENDPOINT_ASYNC](https://oatpp.io/docs/components/api-controller/#endpoint-async-specifics)
