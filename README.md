# 0TZN

Threat model
===========

* File sharing/pasting/website hosting services (pastebin, gist-github, etc...) are not to be trusted with clear text content.
* Data is indexed by search engines
* People constantly scrub these websites to find stuff on it.
* Web surfing logs (URLs) are possibly logged by your ISP/company
* Websurf traffic can be intercepted by bad actors, multiple vuln in TLS 

Here we secure the data using AES running in the browser, and the secret key is in the URL but after the hash marker : it's not leaving your browser.

Threat not covered
-------------------
* Man in the browser, in the os
* Link sharing channel most often poorly secured (typically mail)
