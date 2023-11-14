# MAAS

*November 2023 - v0.0.1*

[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

MAAS (McRib Availability As A Service) provides a modern, RESTful, scalable solution to the common problem of telling people if the popular fast food sandwich is currently available.

Please see https://docs.mcrib.api for API documentation and examples.

# Installation

	npm install

# Run

	npm start

# Test

	npm test

# Docker

	docker build -t maas:1 .
    docker run -v $(pwd):/usr/src/app -p 9000:9000 maas:1

# Clients

API clients are available in a number of languages:

| Language | Name           | Info                                           |
|:---------|:---------------|:-----------------------------------------------|
| JS/Node  | `maas-client` | https://www.npmjs.org/package/maas-client       |

# GUI Clients

| Platform          | Info                                                    |
|:------------------|:--------------------------------------------------------|
| Web               | https://github.com/grahamg/maas                         |

# Contributing

## Adding new operations

To add a new MAAS operation:

1. Fork into your account
2. Branch into a feature branch `feature/your_operation`
3. See the operation files in `/lib/operations`.
4. Add specs, using `/spec/operations` as examples. We won't be merging operations without working specs.
5. Push to your fork and submit a PR.

All contributions are very welcome.
