# Bitcoin knots docker container

**notes:** This project is still under development

## About

Due to request from the [Citadel](github.com/runcitadel/) guys, and also for more client diversity. I've decided to create a docker container for the [Bitcoin Knots implementation](https://github.com/bitcoinknots/bitcoin) for bitcoin.

This is mostly the same, minus a few other differences. You may see the [original project](https://github.com/lncm/docker-bitcoind) which is mostly the same build regime.

## Maintainer notes

### Environment variables

These are used for building and also creating releases in github

- `DOCKER_TOKEN` - docker password or token (for pushing to docker)
- `DOCKER_USER` - docker username (for pushing to docker)
- `GH_PA_TOKEN` - github personal token for creating releases (for pushing to a release)


