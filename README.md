<div style="text-align: center" align="center">
  <img alt="Open Sauced" src="https://i.ibb.co/7jPXt0Z/logo1-92f1a87f.png" width="300px" />

# @open-sauced/semantic-release-conventional-config

> [**semantic-release**](https://github.com/semantic-release/semantic-release) shareable config to publish to `npm` and/or `ghcr`.
> now with alpha and beta pre-releases 

[![Commits](https://img.shields.io/github/commit-activity/w/open-sauced/semantic-release-conventional-config?style=flat)](https://github.com/open-sauced/semantic-release-conventional-config/pulse)
[![Issues](https://img.shields.io/github/issues/open-sauced/semantic-release-conventional-config.svg?style=flat)](https://github.com/open-sauced/semantic-release-conventional-config/issues)
[![Releases](https://img.shields.io/github/v/release/open-sauced/semantic-release-conventional-config.svg?style=flat)](https://github.com/open-sauced/semantic-release-conventional-config/releases)
[![Discord](https://img.shields.io/discord/714698561081704529.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/U2peSNf23P)
[![Twitter](https://img.shields.io/twitter/follow/saucedopen?label=Follow&style=social)](https://twitter.com/saucedopen)

</div>

## 🧪 Plugins

This shareable configuration use the following plugins:

- [`conventional-changelog-conventionalcommits`](https://github.com/conventional-changelog/conventional-changelog)
- [`@semantic-release/commit-analyzer`](https://github.com/semantic-release/commit-analyzer)
- [`@semantic-release/release-notes-generator`](https://github.com/semantic-release/release-notes-generator)
- [`@semantic-release/changelog`](https://github.com/semantic-release/changelog)
- [`@semantic-release/exec`](https://github.com/semantic-release/exec)
- [`@semantic-release/npm`](https://github.com/semantic-release/npm)
- [`@semantic-release/git`](https://github.com/semantic-release/git)
- [`@semantic-release/github`](https://github.com/semantic-release/github)
- [`@semantic-release-plus/docker`](https://github.com/semantic-release-plus/semantic-release-plus/tree/master/packages/plugins/docker)

## 🍕 GitHub actions usage 

Since version 3 it is possible to use semantic-release without any trace of it or the open-sauced configuration anywhere in the dependency tree.

The simplest use case for a typical React application:

```yaml
name: "Release"

on:
  push:
    branches:
      - main

jobs:
  release:
    runs-on: ubuntu-latest
    steps:
      - name: "☁️ checkout repository"
        uses: actions/checkout@v2
        with:
          fetch-depth: 0

      - name: "🚀 release"
        id: semantic-release
        uses: docker://ghcr.io/open-sauced/semantic-release-conventional-config:3.0.0
        env:
          DISABLE_DOCKER: true
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          GIT_AUTHOR_NAME: ${{ github.event.commits[0].author.username }}
          GIT_AUTHOR_EMAIL: ${{ github.event.commits[0].author.email }}
```

## 📦 NPM install and usage

```bash
npm install --save-dev @open-sauced/semantic-release-conventional-config
```

The shareable config can then be configured in the [**semantic-release** configuration file](https://github.com/semantic-release/semantic-release/blob/master/docs/usage/configuration.md#configuration):

```json
{
  "extends": "@open-sauced/semantic-release-conventional-config"
}
```

## 🔧 Configuration

See each [plugin](#plugins) documentation for required installation and configuration steps.

Set `DISABLE_DOCKER` to any value if you want to disable the docker docker plugin.

Set `private` to true in `package.json` if yof want to disable docker.

An example leveraging `node` and `docker` build artifacts can be found in [open-sauced](https://github.com/open-sauced/open-sauced/blob/main/.github/workflows/release.yml).

## 🤝 Contributing

We encourage you to contribute to Open Sauced! Please check out the [Contributing guide](https://docs.opensauced.pizza/) for guidelines about how to proceed.

If you decide to fix a bug, make sure to use the conventional commit available at:

```shell
npm run push
```

<img align="right" src="https://i.ibb.co/CJfW18H/ship.gif" width="200"/>

## 🍕 Community

Got Questions? Join the conversation in our [Discord](https://discord.gg/U2peSNf23P).  
Find Open Sauced videos and release overviews on our [YouTube Channel](https://www.youtube.com/channel/UCklWxKrTti61ZCROE1e5-MQ).

## ⚖️ LICENSE

MIT © [Open Sauced](LICENSE)
