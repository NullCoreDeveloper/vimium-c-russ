<a name="readme"></a><h2 align="center">
  <img src="icons/icon128.png" width="32" height="32" alt="" />
  <span style="color: #2f508e;">Vim</span>ium <span style="color: #a55e18;">C</span> - All by Keyboard (Russified)
</h2>

A customized version of the browser extension for keyboard-based navigation and control.
This version focuses on full Russian localization and improved defaults.

[Читать описание на русском (description in Russian).](README-ru.md)

# Features

* Full keyboard control over web pages
* Contextual mapping
* Global shortcuts
* Command sequences
* Low resource cost (C-style code)

# Keyboard Bindings

Modifier keys are specified as `<c-x>`, `<m-x>`, and `<a-x>` for Ctrl+x, Meta+x, and Alt+x respectively.
For Shift+X and Ctrl+Shift+X, just type `X` and `<c-s-x>`.

Once you have the extension installed, you can see this list of key bindings at any time by typing `?`.

Navigating the current page:

    ?       show the help dialog for a list of all available keys
    h       scroll left
    j       scroll down
    k       scroll up
    l       scroll right
    gg      scroll to top of the page
    G       scroll to bottom of the page
    d       scroll down half a page
    u       scroll up half a page
    f       show hints for links and buttons to open in the current tab
    F       show link hints and open a link in a new tab
    r       reload
    gs      view source
    i       enter insert mode -- all commands will be ignored until you hit Esc to exit
    yy      copy the current url to the clipboard
    yf      copy a link url to the clipboard
    gf      cycle forward to the next frame
    gF      focus the main/top frame

# Building

If you want to compile this project manually, then you need a Node.js 13+ and npm. Please run:

``` bash
npm install typescript
npm install pngjs # only needed for Chromium-based browsers
node scripts/tsc
```

# License

Vimium C: Copyright (c) Gong Dahan and contributors. See the [Apache-2.0 license](LICENSE.txt) for details.
Based on [Vimium](https://github.com/philc/vimium) (MIT license).
