## Usage

copy files and artifacts via SSH as below.

```yaml
name: copy files
on: [push]
jobs:

  build:
    name: Build
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@master
    - name: copy file
      uses: vodapay-gateway/github-action-copy@master
      with:
        source: "tests/a.txt"
        target: "test-a.txt"
```
