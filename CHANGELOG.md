# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog][kac], and this project adheres to
[Semantic Versioning][semver].

[kac]: https://keepachangelog.com/en/1.0.0
[semver]: https://semver.org/spec/v2.0.0.html

## Unreleased

## 0.2.0 - 2021-05-18

### Added

- The client class now has a `headers` property for customizing HTTP headers
  sent in each request. The property can be initialized via the constructor's
  options object (see the [README](README.md#http-headers)).

## 0.1.0 - 2021-05-03

### Added

- Client class for communicating with a Siren server
  - `fetch()` method for hitting API entry point
  - `follow()` method for following links (including embedded links)
  - `submit()` method for submitting actions; currently, only actions whose
    `type` is `"application/x-www-form-urlencoded"` are supported.
- Client `Response` wrapper for parsing Siren responses