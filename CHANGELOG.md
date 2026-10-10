<!-- markdownlint-configure-file { "MD024": { "siblings_only": true } } -->

# Changelog

All notable changes to TokenTracker are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-02-07

First version. The number matches the version the app already reports in
`Info.plist`.

### Added

- A local Python proxy on `localhost:5005` that forwards Anthropic API calls
  unchanged and logs each one's token counts to SQLite. Your API key passes
  through and is never stored.
- Input, output, cache-creation and cache-read tokens per request, with the
  model, endpoint, status code, stop reason and an estimated cost. Streaming
  and non-streaming responses are both tracked.
- A SwiftUI menu bar app showing usage from that database.

[Unreleased]: https://github.com/CleverTrou/TokenTracker/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/CleverTrou/TokenTracker/tree/v1.0.0
