DISCLAIMER: This plugin is not mine.

I only edited a few lines to fix errors and attempted a rough English translation (based on Google Translate):

---

Vim plugin for [XMake](https://github.com/tboox/xmake).

Requires Vim 8.0+ or Neovim.

## Dependencies

* x.vim     https://github.com/luzhlon/x.vim
* qrun.vim  https://github.com/luzhlon/qrun.vim

## Features

* Automatically loads configuration when opening `xmake.lua`
* Reloads configuration when saving `xmake.lua`
* Tab auto-completion(?)
* Asynchronous build; all files will be automatically saved before building
* If the build fails, the quickfix window opens with an error list
* Build and run (open a new cmd window to run under Windows GVim without blocking the GVim window)

## Commands

| Command                 | Description                                               |
| -------------------- | -------------------------------------------------- |
| `:XMake build [target]` | Build target (build all targets if target is not specified)               |
| `:XMake run [target]`   | Run target, if a target is not specified it will attempt to find one   |
| `:XMake [...]`          | Run `xmake` with `...` as parameters, displaying the output in the quickfix window |
| `:XMakeLoad`            | Manually load the configuration in xmake.lua                          |
| `:XMakeGen`             | Generate `xmake.lua` according to the current configuration (experimental)          |
