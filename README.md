# Installation & Usage
Ctags allows jumping to definitions/references. 

Ctags allows you to generate tag files supported by several editors, including [Emacs](https://www.gnu.org/software/emacs/manual/html_node/emacs/Xref.html#Xref), [Vi(m)](https://vim.fandom.com/wiki/Browsing_programs_with_tags) and Atom.

These reg-exes are tested with [universal-ctags](https://github.com/universal-ctags/ctags) (recommended), but should also work with [exuberant-ctags](http://ctags.sourceforge.net/) (unmaintained).

Put the tags definitions in `~/.ctags.d/` or `./.ctags.d/` if you are using *universal-ctags*, or in the file `~/.ctags` or `./.ctags` if using *exuberant-ctags*.

To generate a `TAGS` file for Emacs, run

```
ctags -Re .
```

In the root of the project. I can highly recommend [projectile](https://docs.projectile.mx/en/latest/) which makes this process easier along with many other niceties.

For Vi(m) and Atom, generate a `tags` file by the command

```
ctags -R .
```
