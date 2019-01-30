# Async API Example [![Build Status](https://dev.azure.com/lganzzzo/lganzzzo/_apis/build/status/oatpp.example-async-api?branchName=master)](https://dev.azure.com/lganzzzo/lganzzzo/_build?definitionId=16&branchName=master)

Example project how-to use oatpp asynchronous API.

#### More about oat++:
- Website: [https://oatpp.io](https://oatpp.io)
- Docs: [https://oatpp.io/docs/start](https://oatpp.io/docs/start)
- Oat++ Repo: [https://github.com/oatpp/oatpp](https://github.com/oatpp/oatpp)

## Overview

### Project layout

```

- CMakeLists.txt               // project loader script. load and build dependencies 
- main/                        // main project directory
    |
    |- CMakeLists.txt          // projects CMakeLists.txt
    |- src/                    // source folder
    |- test/                   // test folder
    
```
```
- src/
    |
    |- controller/              // Folder containing controller where all endpoints are declared
    |- dto/                     // DTOs are declared here
    |- AppComponent.hpp         // Service config
    |- Logger.hpp               // Application Logger
    |- App.cpp                  // main() is here
    
```

---

### Build and Run

#### Using CMake

```
$ mkdir build && cd build
$ cmake ..
$ make run        ## Download, build, and install all dependencies. Run project

```

#### In Docker

```
$ docker build -t example-async-api .
$ docker run -p 8000:8000 -t example-async-api
```
