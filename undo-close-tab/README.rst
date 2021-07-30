Undo Close Tab
==============

This was audited by me and cloned from https://github.com/M-Reimer/undoclosetab
at commit 89781768845bfb54c06216568571345747f9a013.

I made the following changes:
 - changed the id in the manifest.json file.

To build, run `make` in this directory and turn off extension signing
(xpinstall.signatures.required: false) in about:config.
