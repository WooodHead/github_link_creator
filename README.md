<p align="center">
  <img alt="GoReleaser Logo" src="src/gopher.jpg" height="100"/>
  <h3 align="center">GitHub Link Card Creater</h3>
  <p align="center">GitHub Link Card Creator lets you generate GitHub images has links to repositories.</p>
</p>

---

<img src="https://img.shields.io/badge/go-v1.11-blue.svg"/> [![CircleCI](https://circleci.com/gh/po3rin/github_link_creator.svg?style=shield)](https://circleci.com/gh/po3rin/github_link_creator) <a href="https://codeclimate.com/github/po3rin/github_link_creator/maintainability"><img src="https://api.codeclimate.com/v1/badges/174111b317186d299133/maintainability" /></a> [![GolangCI](https://golangci.com/badges/github.com/po3rin/github_link_creator.svg)](https://golangci.com)

## Overview

GitHub Link Card Creator lets you generate GitHub images has links to your repositories. This card is useful to guide to your repository in blogs etc.

<a href="https://github.com/po3rin/github_link_creator"><img src="example_card.png" width="460px"/></a>

## Instalation

!! in development ...

using as CLI, you should install folowing command.

```bash
$ go get github.com/po3rin/github_link_creator/cmd/repoimg
```

## Usage

### CLI Mode

!! in development ...

this lets you generate repository card in local.

```bash
repoimg -n po3rin/gotree
```

### Server Mode

set environment valiable ```S3_BUCKET_NAME```. this is target bucket to store image.

```bash
$ go build
$ ./github_link_creator
$ curl localhost:8080/v1/images/<username>/<reponame>
```

When raising the upper limit of API call of GitHub, You should set environment valiable ```GITHUB_CLIRNT_ID``` & ```GITHUB_SECRET```.

> GitHub REST API v3 Documents
> https://developer.github.com/v3/#rate-limiting

## Official CLient

in development ...

https://ghlinkcard.com

## Contributing

You're most welcomed!
Welcome pull request and issues.
