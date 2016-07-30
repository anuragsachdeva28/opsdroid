# Ops Droid

[![Build Status](https://travis-ci.org/opsdroid/opsdroid.svg?branch=master)](https://travis-ci.org/opsdroid/opsdroid) [![Coverage Status](https://coveralls.io/repos/github/opsdroid/opsdroid/badge.svg?branch=master)](https://coveralls.io/github/opsdroid/opsdroid?branch=master)

An open source python chat-ops bot

## Building

`docker build -t opsdroid/opsdroid:dev .`

`docker run --rm opsdroid/opsdroid:dev`

## Configuration

Configuration is done in a yaml file called `configuration.yaml`.

Example:

```
logging: "debug"

connectors:
  shell:

skills:
  hello:
```

## Development

Run tests
`docker run --rm -ti -v $(pwd):/usr/src/app opsdroid/opsdroid:dev tox`