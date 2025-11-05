# Why Use a Copier Template?

Many projects start from some kind of template. These define some basic structure, customized with project specific variables, that developers can add their code into. One example of this is [cookiecutter](https://cookiecutter.readthedocs.io).

The problem with this approach is that it is difficult to apply changes to the template into projects that have been cut from it. Individual changes have to be copy/pasted into the code, leading to partially applied fixes and missed updates.

This template makes use of [copier](https://copier.readthedocs.io/) which gives the best of both worlds, a templating engine to expand the template, then an update mechanism to apply diffs of the updated template to the project.
