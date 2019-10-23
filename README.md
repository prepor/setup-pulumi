# setup-pulumi

Github Action. Install specific version of `pulumi` CLI (http://pulumi.com)

## Usage

```

name: Test

on:
  push:
    branches:    
      - master

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
    - uses: prepor/setup-pulumi@master
      with:
        version: 1.3.4
    - run: pulumi version
```
