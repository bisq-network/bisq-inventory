# bisq-inventory

## Overview

For checking the health of the Bisq seed nodes from a browser, e.g., http://localhost:8080

## Building source code

This repo has a dependency on git submodule [bisq](https://github.com/bisq-network/bisq).  
There are two ways to clone it before it can be compiled:

```
# 1) Use the --recursive option in the clone command:
$ git clone --recursive  https://github.com/bisq-network/bisq-inventory.git

# 2) Do a normal clone, and pull down the bisq repo dependency with two git submodule commands:
$ git clone https://github.com/bisq-network/bisq-inventory.git
$ cd bisq-inventory
$ git submodule init
$ git submodule update
```

To build:
```
$ ./gradlew clean build
```
