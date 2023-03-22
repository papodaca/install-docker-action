# Usage

Use like this:

```yml
name: build
run-name: build images
on: [push]
jobs:
  local-registry:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v3
      - name: Install docker
        uses: papodaca/install-docker-action@main
```