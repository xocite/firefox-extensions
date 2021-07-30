firefox-extensions
==================
A selection of Firefox extensions that I've audited and modified for my own use.

- `close-tab`: closes the current tab
- `undo-close-tab`: undoes the last closed tabs up to 25 previous tabs
- `list-tab`: lists the currently open tabs

I primarily use these with the following userChrome.js modifications which hide
the tab bar at the top.  I use this configuration with Ctrl-Tab and "don't open links in new
tabs" setting in Firefox preferences.::

  #tabbrowser-tabs {
  	visibility: collapse !important;
  }

To install these extensions you'll either have to install them temporarily via
`about:debugging` as a temporary add-on or install Firefox Developer Edition or
Nightly and install directly from `about:addons`.
