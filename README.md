# Standard .NET Project Layout

## Overview

This is a basic layout for .NET application projects. It's **`not an official standard defined by .NET team`**. However, it is a set of common historical and emerging project layout patterns in the .NET ecosystem. Some of these patterns are more popular than others. It's combining from https://gist.github.com/davidfowl/ed7564297c61fe9ab814 and https://github.com/golang-standards/project-layout


## .NET Directories

## `/src`

Your main project to start coding.

See the [`/src`](src/README.md) directory for examples.

### `/build`

Build customizations, packaging and CI

See the [`/build`](build/README.md) directory for examples.


### `/scripts`

Scripts to perform various install, analysis, etc operations.

These scripts can be combine with `Makefile` in the root level.

See the [`/scripts`](scripts/README.md) directory for examples.

### `/deployments`

IaaS, PaaS, system and container orchestration deployment configurations and templates (docker-compose, kubernetes/helm, mesos, terraform, bosh). Note that in some repos (especially apps deployed with kubernetes) this directory is called `/deploy`.

### `/tests`

Unit test and integration test of your projects. Feel free to structure the `/test` directory anyway you want. 

See the [`/tests`](tests/README.md) directory for examples.

## Other Directories

### `/docs`

Design and user documents

See the [`/docs`](docs/README.md) directory for examples.

### `/examples` (optional)

Examples for your applications and/or public libraries.

See the [`/examples`](examples/README.md) directory for examples.

### `/packages`

Contains NuGet packages
