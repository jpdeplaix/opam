Working version changelog, used as a base for the changelog and the release
note.
Possibly scripts breaking changes are prefixed with ✘.
New option/command/subcommand are prefixed with ◈.

## Version
  *

## Global CLI
  *

## Init
  *

## Config Upgrade
  *

## Install
  *

## Remove
  *

## Switch
  *

## Pin
  *

## List
  *

## Show
  *

## Var
  *

## Option
  *

## Lint
  *

## Lock
  *

## Opamfile
  * Fix `features` parser [#4507 @rjbou]

## External dependencies

## Sandbox
  *

## Repository management
  *

## VCS
  *

## Build
  * Fix opam-devel's tests on platforms without openssl, GNU-diff and a system-wide ocaml [#4500 @kit-ty-kate]

## Infrastructure
  *

## Admin
  *

## Opam installer
  *

## State
  *

# Opam file format
  *

## Solver
  * Add bultin support for the 'deprecated' flag.
    Any packages flagged with deprecated would be avoided by the solver unless there is no other choice (e.g. some user wants to install package a which depends on b which is deprecated)
    If it is installed, show up a note after installation notifying the user that the package is deprecated.
    [#4523 @kit-ty-kate]

## Client
  *

## Internal
  *

## Test
  *

## Shell
  *

## Doc
  * Install page: add OSX arm64 [#4506 @eth-arm]
  * Document the default build environment variables [#4496 @kit-ty-kate]
