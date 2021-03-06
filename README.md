Emacs-SMBC
==========

The fun (and the copyright) credits go to [SMBC](http://smbc-comics.com/) of course!

Emacs-SMBC is an Emacs plugin to help you (Save the world? Sadly no) read SMBC without leaving your Emacs!

It is planned to have a lot of functions to make reading SMBC easier.

### Installation:
If you don't have Melpa configured already, put this in your `.emacs` or `init.el`:
```lisp
(when (>= emacs-major-version 24)
  (require 'package)
  (add-to-list
   'package-archives
   '("melpa" . "http://melpa.org/packages/")
   t)
  (package-initialize))
```

Then follow it up with `M-x package-install` and enter `smbc` in the following prompt.
  
### Usage
Simply load the file (place it in your `.emacs.d` and load it, or else use `M-x load-file` and give its path).<br>
Better still, add it to your `init.el`, it's easy and fast to load.

Access the latest comic with `M-x smbc-get-latest`.

View the previous comic with `C-c p` inside the smbc buffer, or go forward one using `C-c n`.

### Misc
On MELPA as `smbc` [here](https://github.com/sakshamsharma/melpa/blob/master/recipes/smbc)

Reddit discussion [here](https://www.reddit.com/r/emacs/comments/4lrjln/a_simple_smbc_viewer_for_emacs/)

### TODO

* Check for new comics every time on startup
* Cache last few comics
* Allow opening comic in browser
* Use RSS feed instead of parsing HTML
* Read some more SMBC :smile:
