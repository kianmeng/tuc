# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),

## [Unreleased]

- feat: smaller binaries by removing unnecessary (to us) regex features

## [0.11.0] - 2022-06-20

- fix: --lines could throw out of bounds with -f 1: in some situations
- chore: dependency updates
- doc: fixed typos
- doc: new section about community-managed install methods (macports)
- doc: man page generated using the mode modern pandoc 2.5

## [0.10.0] - 2022-06-13

- breaking: -E is now an option (-e), and accept the regex as value
- doc: added man page
- doc: improved documentation
- chore: updated pico-args

## [0.9.0] - 2022-06-05

- breaking: --lines output each bound on their own line
- feat: --regex support
- feat: minor tuning of buffers
- feat: internal improvements for --lines
- fix: right side of a range can be negative
- fix: emit proper error if right side of a range is behind left side
- fix: --lines with negative indexes were broken
- fix: --greedy-delimiter was cutting wrongly lines starting with delimiter

## [0.8.0] - 2022-05-23

- Add support for --greedy-delimiter
- Bounds can be formatted
- Major refactoring for better code maintainability

## [0.7.0] - 2022-05-21

- Add support for --join
- Add support for --lines
- Add support for --complement
- Add support for --zero-terminated

## [0.6.0] - 2022-05-13

- Add split-by-byte using --bytes
- Add split-by-character using --characters
- Faster performance when -p (compress delimiters) is on
- Faster performance when reading the input
- CI now fails if the linter is not satisfied
- Reviewd CI/release actions, simpler, faster
- Release binaries for ARM too

## [0.5.0] - 2021-07-21

- Better performances (faster, less allocations)
- Faster to compile
- Smaller binary size
- Display a better error message on unknown arguments
- Add an option to get the version back
- Migrate to pico-args
- Fix output when --only-delimited is present
- Delimiters are replaced once, allowing empty strings
- Updated dependencies
- More integration tests

## [0.4.0] - 2020-05-31

### Changed
- Build binaries for multiple operative systems
- Fixed typos in the documentation

## [0.3.0] - 2020-05-31

### Changed
- More examples
- New releases system

## [0.2.0] - 2020-05-30

### Added

- Option -p has now a long version, "compress-delimiter"

## [0.1.0] - 2020-05-30

### Added

- Can cut given a (multi)character delimiter
- Can compress the delimiter in the output
- Can replace the delimiter in the output with a string
- Can omit lines not matching delimiters
