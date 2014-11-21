OSULUG-Website
==============

[![Build
Status](https://travis-ci.org/OSULUG/OSULUG-Website.svg?branch=master)](https://travis-ci.org/OSULUG/OSULUG-Website)

Website for the Linux User's Group of Oregon State University

Modifying the website: 
----------------------

Fork the project or just clone a copy. To add content, add or edit the markdown files in the content directory. 

Markdown explanation is at http://daringfireball.net/projects/markdown/

Testing changes:
----------------

```
$ cd OSULUG-Website
$ virtualenv venv                   # only the first time
$ source venv/bin/activate
$ pip install -r requirements.txt   # only the first time and if the reqs change
$ wok --server
$ deactivate

```

More info about wok is at http://wok.mythmon.com/

Getting it Online: 
------------------

Once you've made and tested your changes, submit a pull request and then ping edunham about it. 

We need to eventually set up a post-commit hook to get the machine hosting lug.oregonstate.edu to 
automatically pull from this repo and run wok whenever code gets committed here. Until then, just 
have someone with the necessary access (probably edunham) do it manually.
