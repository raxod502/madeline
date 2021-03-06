# Changelog

All notable changes to this project will be documented in this file.
The format is based (loosely) on [Keep a Changelog].

[keep a changelog]: http://keepachangelog.com/

## 1.0.2 (released 2019-02-12)
### Fixed
* Previously, Madeline died with a traceback saying `TypeError:
  write() argument must be str, not None` when used with incorrect
  command-line arguments, under some circumstances. This has now been
  fixed.
* The usefulness of Madeline's `--verbose` progress messages has been
  improved. Previously, in some circumstances, the parent directory of
  a file would be displayed while the file was being transferred,
  instead of the file itself. This has been fixed.

## 1.0.1 (released 2018-09-08)
### Fixed
* Previously, if Madeline encountered an error or warning while
  mirroring verbosely, the error or warning message would be
  distastefully interspersed with the verbose status messages. This
  has been fixed, and now acts the way you would expect.

## 1.0 (released 2018-08-01)
### Added
* Python package: `madeline`
* Binary: `madeline`
  * Command-line arguments:
    * `--source`
    * `--target`
    * `put | get`
    * `--exclude`
    * `--verbose | --no-verbose`
    * `--identity | --no-identity`
    * `--ssh-add | --no-ssh-add`
  * Environment variable: `MADELINE_DEBUG`
