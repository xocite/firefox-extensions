Close Tab
=========

This was audited by me and cloned from https://github.com/codefisher/toolbar_buttons at commit
534e5b1c39150b769107957d5f2a38726fda7ac8.

I made the following changes:
 - pulled out the close tab functionality and icon
 - created the extension files
 - added the close icon from Feather icons https://github.com/feathericons/feather/tree/v4.28.0

To build, run `make` in this directory and turn off extension signing
(xpinstall.signatures.required: false) in about:config.
