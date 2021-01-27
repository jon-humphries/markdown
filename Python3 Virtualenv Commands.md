# Python3 Virtualenv Commands


This page highlights how to setup and use virtualenv on the MACOS.

A Virtual Environment, is an isolated working copy of Python which allows you to work on a specific project without affecting other projects by installing or disrupting various dependencies.

It enables multiple side-by-side installations of Python, one for each project.

You can install modules etc without conflicting with the global python install.


To install virtualenv:

`pip3 install virtualenv`

To begin using virtualenv first create a directory for the isolated environment:

`mkdir ~/virtualenv/new_app`

To create a folder for your new app that includes a clean copy of Python run:


`python -m venv new_app`

(add –no-site-packages if you want to isolate your environment from the main site
packages directory)

To begin working with your project, you have to cd into your directory (project)
and activate the virtual environment.

Lastly, activate your environment:

`source /Users/path_user/virtualenv/new_app/bin/activate`

Notice how the prompt of your shell changed to show the active environment.

`(new_app) users@MacBook ~ %`

That is how you can see that you’re in your new environment.


Any packages you install now using pip or easy_install get installed into new_app/lib/python3.x/site-packages.

`To exit your virtualenv just type “deactivate”.`


