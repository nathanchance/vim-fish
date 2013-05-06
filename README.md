vim-fish
========

This is an addon for Vim providing filetype support for [fish][] scripts.  In
addition to the normal Vim features such as syntax highlighting, automatic
indentation and filetype detection, this addon includes support for the
third-party addons [UltiSnips][], [Syntastic][], [endwise][] and [commentary][]
when any of those are installed.  Bonus feature: if you use Vim with `funced`
in fish the cursor will be placed inside the function and Vim will enter Insert
mode.

[fish]: https://github.com/fish-shell/fish-shell
[UltiSnips]: https://github.com/SirVer/ultisnips
[Syntastic]: https://github.com/scrooloose/syntastic
[endwise]: https://github.com/tpope/vim-endwise
[commentary]: https://github.com/tpope/vim-commentary


Using fish with Vim
-------------------

Vim needs a more POSIX compatible shell than fish for certain functionality to
work, such as `:%!`, compressed help pages and many third-party addons.  If you
use fish as your login shell or launch Vim from fish, you need to set `shell`
to something else in your `~/.vimrc`, for example:

```vim
set shell=/bin/sh
```

Best do it somewhere at the top, before any addon code is loaded and executed.