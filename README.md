# esa.el --- Interface to esa.io (\\( ⁰⊖⁰)/)
## Installation

    $ cd ~/.emacs.d/vendor
    $ git clone git://github.com/nabinno/esa.el.git

In your emacs config:

```lisp
(add-to-list 'load-path "~/.emacs.d/vendor/esa.el")
(require 'esa)
```

## Functions

- `M-x esa-list` - Lists your esas in a new buffer. Use arrow keys to
  browse, RET to open one in the other buffer.
- `M-x esa-search` - Search queries and lists your esas in a new buffer.
- `M-x esa-region` - Copies esa URL into the kill ring.  With a prefix
  argument, ships a esa.
- `M-x esa-region-wip` - Explicitly create a esa on WIP.
- `M-x esa-buffer` - Copies esa URL into the kill ring.  With a
  prefix argument, ships a esa.
- `M-x esa-buffer-private` - Explicitly create a esa on WIP.
- `M-x esa-region-or-buffer` - Post either the current region, or if
  mark is not set, the current buffer as a new paste at
  yourteam.esa.io.  Copies the URL into the kill ring.  With a prefix
  argument, ships a esa.
- `M-x esa-region-or-buffer-wip` - Explicitly create a esa from the
  region or buffer.

## Configuration
### OAuth authentication

Get the `Personal API Access Token` from:

https://yourteam.esa.io/user/tokens

Put following to your .emacs:

```lisp
(setq esa-token "******************************")
(setq esa-team-name "yourteam")
```

### Other customizations

    M-x customize-group (esa)

---

## Meta

* Code: `git clone git://github.com/nabinno/esa.el.git`
* Home: <https://github.com/nabinno/esa.el>
* Bugs: <https://github.com/nabinno/esa.el/issues>
* Hosting: melpa

## EPILOGUE

>     A whale!
>     Down it goes, and more, and more
>     Up goes its tail!
>
>     -Buson Yosa
