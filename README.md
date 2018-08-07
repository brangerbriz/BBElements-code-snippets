# BBElements Code Snippets

[BBElements](https://github.com/brangerbriz/BBElements) code snippets for VS Code and Atom editors.

## Installing

The installation process is different dependent on which editor you are using.

### VS Code

```bash
curl -o ~/.config/Code/User/snippets/bbelements.code-snippets  https://raw.githubusercontent.com/brangerbriz/BBElements-code-snippets/master/vscode/bbelements.code-snippets
```

At the time of this writing `~/.config/Code/User/snippets/` is the snippets directory for VS Code on Linux. If you are using another operating system save the `bbelements.code-snippets` in whatever folder snippets are normally saved in.

### Atom

Atom saves all user defined snippets in one file, so it's probably safer to copy + paste [this file](https://raw.githubusercontent.com/brangerbriz/BBElements-code-snippets/master/atom/snippets.cson) into your editor's `snippets.cson` file rather than overwriting it and clobbering your existing snippets. On linux this file lives in `~/.atom/snippets.cson`.

See the [Atom snippets documentation](https://flight-manual.atom.io/using-atom/sections/snippets/) for more info.

## Usage

These code snippets support all tag types specified in the [BBElements README](https://github.com/brangerbriz/bbelements). Here is a list of the snippet names:

- bb.css
- bb.scripts
- bb.logo
- bb.h1
- bb.h2
- bb.h3
- bb.tags
- bb.date
- bb.marginal-note
- bb.quote
- bb.media-block
- bb.media-inline
- bb.code

### VS Code

CTRL + SPACE activates your list of snippets, press TAB or ENTER to select ones. BBElement snippets use the `bb.*` namespace. Once you have selected the snippet, pressing TAB will jump between autofill parameters if the snippet includes any.

### Atom

Atom snippets are enabled by default for and should be autosuggested as you type. The BBElements code snippets are named like `bb.*`, however in Atom, typing the "." key restarts the snippet autocomplete. You can replace the "." with "-" while specifying your snippet to account for this (e.g. type `bb-quote` and `bb-media-block` instead of `bb.quote` and `bb.media-block`). Press TAB or ENTER to select a snippet once it is suggested. Once you have selected the snippet, pressing TAB will jump between autofill parameters if the snippet includes any.

BBElements snippets are only supported in files with the `.html` and `.md` file extension.
