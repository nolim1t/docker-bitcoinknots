# Bitcoin knots docker container

**notes:** This project is still under development

[![Build Status]][builds]
[![gh_last_release_svg]][gh_last_release_url]
[![Docker Pulls Count]][bitcoinknots-docker-hub]

[builds]: https://github.com/nolim1t/docker-bitcoinknots/actions?query=workflow%3A%22Build+%26+deploy+on+git+tag+push%22
[Build Status]: https://github.com/nolim1t/docker-bitcoinknots/workflows/Build%20&%20deploy%20on%20git%20tag%20push/badge.svg

[gh_last_release_svg]: https://img.shields.io/github/v/release/nolim1t/docker-bitcoinknots?sort=semver
[gh_last_release_url]: https://github.com/nolim1t/docker-bitcoinknots/releases/latest

[Docker Pulls Count]: https://img.shields.io/docker/pulls/nolim1t/bitcoinknots.svg?style=flat
[bitcoinknots-docker-hub]: https://hub.docker.com/r/nolim1t/bitcoinknots


## About

Due to request from the [Citadel](github.com/runcitadel/) guys, and also for more client diversity. I've decided to create a docker container for the [Bitcoin Knots implementation](https://github.com/bitcoinknots/bitcoin) for bitcoin.

This is mostly the same, minus a few other differences. You may see the [original project](https://github.com/lncm/docker-bitcoind) which is mostly the same build regime.

### Todo list

- [x] Add option to push to **any** docker hub user in environment variables
- [ ] Improve on workflow
- [ ] Move over to LNCM org so that

### Diferences

I've removed the verification component, but ideally I'd like to be able to verify releases the same way as I do with bitcoin core. If anyone has a PGP key that I could verify for the sources in github please let me know. It's good to have a healthy paranoia when dealing with finances.

## Maintainer notes

### Environment variables

These are used for building and also creating releases in github

- `DOCKER_HUB_USER` - docker hub user to push to. Permissions MUST be correct or it will fail.
- `DOCKER_TOKEN` - docker password or token (for pushing to docker)
- `DOCKER_USER` - docker username (for pushing to docker)
- `GH_PA_TOKEN` - github personal token for creating releases (for pushing to a release)


