Working version changelog, used as a base for the changelog and the release
note.
Possibly scripts breaking changes are prefixed with ✘
New option are prefixed with ◈

## Admin
  * Fix admin cache synchronisation message [#4193 @rjbou - fix #4167]

## Init
  * Remove m4 from the list of recommended tools [#4184 @kit-ty-kate]
  * Fix config solver field ignored [#4243 @rjbou - fix #4241]

## Switch
  * Fix Not_found with `opam switch create . --deps` [#4151 @AltGr]

## Upgrade
  * Fix atoms formula restriction with `--all` [#4221 @rjbou - fix #4218]

## Build
  * Opam file build using dune, removal of opam-%.install makefile target [#4178 @rjbou #4229 @kit-ty-kate - fix #4173]
  * Use version var in opam file instead of equal current version number in opamlib dependencies [#4178 @rjbou]
  * ext: fix extlib url [#4248 @rjbou]
  * Bump to alpha2 version [#4253 @rjbou]

## Install
  * Add `_build` to rsync exclusion list [#4230 @rjbou - fix #4195]
  * Recursive opam file lookup: ignore `_build` [#4230 @rjbou]
  * Assume-built fix & rewriting [#4211 @rjbou]

## Archives fetch
  * Copy instead of calling rsync when archives are in a local cache [#4270 @kit-ty-kate]

## Switch
  * Fix Not_found with `opam switch create . --deps` [#4151 @AltGr]
  * Package Var: resolve self `name` variable for orphan packages [#4228 @rjbou - fix #4224]
  * ✘ Reject (shell) character on switch names [#4237 @rjbou - fix #4231]
  * Add missing depext to unavailable reasons [#4194 @rjbou - fix #4176]
    * Fix not found error [#4279 @rjbou]


## Pin
  * Add depext handling on new pinned packages [#4194 @rjbou - fix #4189]

## Option
  * Fix messages advertising a command in an obsolete format [#4194 @rjbou]

## Config
  * Add switch depext-bypass as modifiable field [#4194 @rjbou - fix #4177]

## List
  * Add --no-depexts option to disable depexts packages unavailability [#4194 @rjbou - fix #4205]
  * Warn if packages are not listed because of depexts unavailaibilty [#4194 @rjbou - fix #4205]

## Pin
  * Don't keep unpinned package version if it exists in repo [#4073 @rjbou - fix #3630]
  * Fix path resolving when pinning with `file://` [#4209 @rjbou - fix #4208]
  * ✘ Disable recursive & subpath pinning (only present experimentally in opam 2.1.0~alpha) [#4252 @rjbou]

## Show
  * ✘ Display error message for all not found packages [#4179 @rjbou - fix #4164]
  * ✘ Keep package order given via cli [#4179 @rjbou - fix #4163]
  * `--sort`` apply to with all options, not only `--just-file` [#4179 @rjbou]

## Lint
  * E65: check that url local path ar absolute [#4209 @rjbou]

## Depext
  * Fix arch query [#4200 @rjbou]
  * Add message when adding a package to `depext-bypass` [#4194 @rjbou]
  * Fix performance issue of depext under Docker/debian [#4165 @AltGr]
  * Refactor package status [#4152 #4200 @rjbou]
  * Add environment variables handling [#4200 @rjbou]
  * Add Macport support [#4152 @rjbou]
  * Homebrew: add no auto update env var for install, accept `pkgname` and `pkgnam@version` on query [#4200 @rjbou]
  * Tag packages with missing depexts in Cudf [#4235 @AltGr]
  * Force LC_ALL=C for query commands [#4200 @rjbou]
  * Put back opam-depext-2.0's behaviour with regards to asking users' consent before installing system packages [#4168 @kit-ty-kate @rjbou]
  * Add OPAMDEPEXTYES env variable to pass --yes options to system package manaer [#4168 @kit-ty-kate @rjbou]
  * Fix install command dryrun [#4200 @rjbou]
  * ◈ Add --depext-only to install only external dependencies, regardless of config depext status [#4238 @rjbou]
  * Move confirmation message after opam packages install [#4238 @rjbou]
  * Error if '--depext-only' is given with '--assume-depexts' or '--no-depexts'
  * Handle debian virtual packages [#4269 @AltGr @rjbou - fix #4251]

## Var
  * Not found message show scope [#4192 @rjbou]
  * No scope needed for variable display [#4192 @rjbou - fix #4183]
  * Fix package variable resolution [#4192 @rjbou - fix #4182]

## Repository management
  * Fix temp files repository cleaning [#4197 @rjbou]

## Env
  * Fix `OPAMSWITCH` empty string setting, consider as unset [#4237 @rjbou]

## Sandbox
  * No error when linked directory doesn't exist (e.g. XDG defined) [#4278 @kit-ty-kate]
  * Add quotew to avoid space unwanted behaviors [#4278 @kit-ty-kate]

## Remove
  * Fix autoremove env var handling [#4219 @rjbou - fix #4217]

## Repository management
  * Fix temp files repository cleaning [#4197 @rjbou]

## Opam installer
  * For paths, remove use of empty switch in favor of a context-less module [#4237 @rjbou]

## Internal
  * Disable chrono when timestamps are disables [#4206 @rjbou]
  * Expose some functionality in the `OpamAction`, `OpamPath` and `OpamSwitchState`
    modules for use without a `switch` value [#4147 @timberston]
    * Path: introduce a functor to permit replicating switch layout in different contexts
  * Std: Add map_reduce to Set and Map [#4263 @AltGr]

## Solver
  * Fix Cudf generation for compat with external solvers [#4261 @AltGr]
  * Check for a solution before calling the solver [#4263 @AltGr]

## Test
  * Add show cram test [#4206 @rjbou]
  * Add envrionnement variable handling on cram test [#4206 @rjbou]

## Doc
  * add doc/warning for  Filename.rmdir_cleanup [#4197 @rjbou]
  * add badges to install page [#4236 @rjbou]
  * Harden build system against changing the name of the opam binary [#4264 @dra27]
  * Fix typo [#4273 @robz]
  * Remove recursive & subpath pinning doc [#4252 @rjbou]

## Var
  * Not found message show scope [#4192 @rjbou]
  * No scope needed for variable display [#4192 @rjbou - fix #4183]
  * Fix package variable resolution [#4192 @rjbou - fix #4182]

## Infrastructure
  * Use OCaml 4.09.1 for the make cold target [#4257 @dra27]

## Opam file
  * Fix mismatching extra files detection [#4198 @rjbou]
