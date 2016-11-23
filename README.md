# Flycheck plantuml Checker

[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)
[![MELPA](http://melpa.org/packages/flycheck-plantuml-badge.svg)](http://melpa.org/#/flycheck-plantuml)
[![Build Status](https://travis-ci.org/alexmurray/flycheck-plantuml.svg?branch=master)](https://travis-ci.org/alexmurray/flycheck-plantuml)

Integrate [plantuml](http://plantuml.com)
(via [plantuml-mode](https://github.com/skuro/plantuml-mode))
with [flycheck](http://www.flycheck.org) to automatically check the syntax of
your plantuml files on the fly.

## Installation

### MELPA

The preferred way to install `flycheck-plantuml` is
via [MELPA](http://melpa.org) - then you can just <kbd>M-x package-install RET
flycheck-plantuml RET</kbd>

To enable then simply add the following to your init file:

```emacs-lisp
(with-eval-after-load 'flycheck
  (require 'flycheck-plantuml)
  (flycheck-plantuml-setup))
```

### Manual

If you would like to install the package manually, download or clone it and
place within Emacs' `load-path`, then you can require it in your init file like
this:

```emacs-lisp
(require 'flycheck-plantuml)
(flycheck-plantuml-setup)
```

NOTE: This will also require the manual installation of `flycheck` and
`plantuml-mode` if you have not done so already.

## License

Copyright © 2016 Alex Murray

Distributed under GNU GPL, version 3.
