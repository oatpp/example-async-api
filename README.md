# Async API Example [![Build Status](https://dev.azure.com/lganzzzo/lganzzzo/_apis/build/status/oatpp.example-async-api?branchName=master)](https://dev.azure.com/lganzzzo/lganzzzo/_build?definitionId=16&branchName=master)

Example project how-to use oatpp asynchronous API.

#### More about oat++:
- Website: [https://oatpp.io](https://oatpp.io)
- Docs: [https://oatpp.io/docs/start](https://oatpp.io/docs/start)
- Oat++ Repo: [https://github.com/oatpp/oatpp](https://github.com/oatpp/oatpp)

## Overview

### Project layout

```
- CMakeLists.txt                        // projects CMakeLists.txt
- src/
    |
    |- controller/                      // Folder containing controller where all endpoints are declared
    |- dto/                             // DTOs are declared here
    |- AppComponent.hpp                 // Service config
    |- Logger.hpp                       // Application Logger
    |- App.cpp                          // main() is here

- test/                                 // test folder
- utility/install-oatpp-modules.sh      // utility script to install required oatpp-modules.
    
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
