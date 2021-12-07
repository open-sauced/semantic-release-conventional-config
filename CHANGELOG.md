# 📦 open-sauced/semantic-release-conventional-config changelog

[![conventional commits](https://img.shields.io/badge/conventional%20commits-1.0.0-yellow.svg)](https://conventionalcommits.org)
[![semantic versioning](https://img.shields.io/badge/semantic%20versioning-2.0.0-green.svg)](https://semver.org)

> All notable changes to this project will be documented in this file

## [3.1.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v3.0.1...v3.1.0) (2021-12-07)


### 📝 Documentation

* update readme with latest action enhancements and fix previous changelog header artifacts ([#27](https://github.com/open-sauced/semantic-release-conventional-config/issues/27)) ([5c52b76](https://github.com/open-sauced/semantic-release-conventional-config/commit/5c52b765a4e6c2869904f4851247d950f5119466))

### [3.0.1](https://github.com/open-sauced/semantic-release-conventional-config/compare/v3.0.0...v3.0.1) (2021-12-05)


### 🐛 Bug Fixes

* correct license plugin and refactor all tooling ([#26](https://github.com/open-sauced/semantic-release-conventional-config/issues/26)) ([dc9a109](https://github.com/open-sauced/semantic-release-conventional-config/commit/dc9a1092d86e25824dd02c5fcfd87d778c1caef0)), closes [#25](https://github.com/open-sauced/semantic-release-conventional-config/issues/25)

## [3.0.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v2.1.0...v3.0.0) (2021-12-04)


### ⚠ BREAKING CHANGES

* it is no longer required to install this package as part of your NPM tooling as
long as you are using GitHub Actions
* marketplace integration works now but it needs a manual verification for every tag we want to list, the major tag updates being handled by another action when we edit the GitHub release

### Features

* dockerize repository and release package on ghcr.io ([#21](https://github.com/open-sauced/semantic-release-conventional-config/issues/21)) ([847456e](https://github.com/open-sauced/semantic-release-conventional-config/commit/847456ec3c7bc7cb46ad8acbcb311934f60a5445)), closes [#18](https://github.com/open-sauced/semantic-release-conventional-config/issues/18) [#11](https://github.com/open-sauced/semantic-release-conventional-config/issues/11) [#24](https://github.com/open-sauced/semantic-release-conventional-config/issues/24) [#24](https://github.com/open-sauced/semantic-release-conventional-config/issues/24)

## [2.1.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v2.0.4...v2.1.0) (2021-11-10)


### Features

* implement @open-sauced/conventional commit ([#20](https://github.com/open-sauced/semantic-release-conventional-config/issues/20)) ([0ce2853](https://github.com/open-sauced/semantic-release-conventional-config/commit/0ce28530b2d7d2d364aded6745bd1ac632391fcb)), closes [#19](https://github.com/open-sauced/semantic-release-conventional-config/issues/19)

### [2.0.4](https://github.com/open-sauced/semantic-release-conventional-config/compare/v2.0.3...v2.0.4) (2021-11-06)


### Continuous Integration

* improve workflow reusability across repositories ([#17](https://github.com/open-sauced/semantic-release-conventional-config/issues/17)) ([509fb0c](https://github.com/open-sauced/semantic-release-conventional-config/commit/509fb0c85404827db45c5d4a81fa43c0f524495f))

### [2.0.3](https://github.com/open-sauced/semantic-release-conventional-config/compare/v2.0.2...v2.0.3) (2021-11-01)


### Bug Fixes

* correct uppercase usernames and repos, fix typo in npm package release ([#15](https://github.com/open-sauced/semantic-release-conventional-config/issues/15)) ([9c7d3aa](https://github.com/open-sauced/semantic-release-conventional-config/commit/9c7d3aafcbaa3495254e478ff1f7de367024fef0)), closes [#12](https://github.com/open-sauced/semantic-release-conventional-config/issues/12)

### [2.0.2](https://github.com/open-sauced/semantic-release-conventional-config/compare/v2.0.1...v2.0.2) (2021-11-01)


### Bug Fixes

* add package lock to semantic release git configuration ([#14](https://github.com/open-sauced/semantic-release-conventional-config/issues/14)) ([90c9e8c](https://github.com/open-sauced/semantic-release-conventional-config/commit/90c9e8cfe1f619aadd53cd2d86001a816a4d9e52)), closes [#13](https://github.com/open-sauced/semantic-release-conventional-config/issues/13)

### [2.0.1](https://github.com/open-sauced/semantic-release-conventional-config/compare/v2.0.0...v2.0.1) (2021-10-25)


### Bug Fixes

* correct ci docker login variables ([#10](https://github.com/open-sauced/semantic-release-conventional-config/issues/10)) ([f1dfac0](https://github.com/open-sauced/semantic-release-conventional-config/commit/f1dfac0a1853e5e18703d7e95f0b257017a339ff))

## [2.0.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.4.0...v2.0.0) (2021-10-25)


### ⚠ BREAKING CHANGES

* node-version: the minimum required version of node is now v14.17

### Features

* update to node@14 ([#9](https://github.com/open-sauced/semantic-release-conventional-config/issues/9)) ([b4a6015](https://github.com/open-sauced/semantic-release-conventional-config/commit/b4a6015c929d271e34411f560f745b6474cc351a))

## [1.4.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.3.0...v1.4.0) (2021-10-10)


### Features

* implement @open-sauced/check-engines ([#8](https://github.com/open-sauced/semantic-release-conventional-config/issues/8)) ([ea81503](https://github.com/open-sauced/semantic-release-conventional-config/commit/ea8150315e8897177a6f461f053c2c8ee53f9192))

## [1.3.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.2.0...v1.3.0) (2021-10-03)


### Features

* add diagram for opensauced githubocto/repo-visualizer implementation ([#7](https://github.com/open-sauced/semantic-release-conventional-config/issues/7)) ([055a9f7](https://github.com/open-sauced/semantic-release-conventional-config/commit/055a9f718cc7679863d6b4d9952ee0397128da03))

## [1.2.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.1.1...v1.2.0) (2021-08-11)


### Documentation

* add some workflow clarifications ([#6](https://github.com/open-sauced/semantic-release-conventional-config/issues/6)) ([8755089](https://github.com/open-sauced/semantic-release-conventional-config/commit/87550891492cb812a29d4a3e4ed63ba561a4ae06)), closes [#3](https://github.com/open-sauced/semantic-release-conventional-config/issues/3)

### [1.1.1](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.1.0...v1.1.1) (2021-08-11)


### Continuous Integration

* add open-sauced triage wonkflows ([#5](https://github.com/open-sauced/semantic-release-conventional-config/issues/5)) ([2cb3889](https://github.com/open-sauced/semantic-release-conventional-config/commit/2cb388954216097f3dfbe7de48bfbb4920b34735)), closes [#4](https://github.com/open-sauced/semantic-release-conventional-config/issues/4)

## [1.1.0](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.0.1...v1.1.0) (2021-07-31)


### Documentation

* correct install procedure ([165075a](https://github.com/open-sauced/semantic-release-conventional-config/commit/165075a5556d442037aa053e800928e300a7b837))

### [1.0.1](https://github.com/open-sauced/semantic-release-conventional-config/compare/v1.0.0...v1.0.1) (2021-07-31)


### Bug Fixes

* proper package public scope on publish config ([0bca8fa](https://github.com/open-sauced/semantic-release-conventional-config/commit/0bca8faa4b44e82517eb3d26d4e91e30f67241cf))

## 1.0.0 (2021-07-31)


### Features

* initial commit ([2f02692](https://github.com/open-sauced/semantic-release-conventional-config/commit/2f02692c1cae0e834bfe9a3d0b6303c3a9e17d82))


### Continuous Integration

* add minimal release workflow ([bbaa891](https://github.com/open-sauced/semantic-release-conventional-config/commit/bbaa891c450fe83610ce709ed4ebc125ea6775b6))
