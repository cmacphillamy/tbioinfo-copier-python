# Adopt the template into an existing repo

You can adopt this template into an existing repo by running `copier copy` in much the same way as in a new project.

This will:

- Ask some questions about the existing project
- Expand the template with the answers given
- Ask if you would like to overwrite conflicting files (always choose yes)
- Record the answers in the project so they can be used in later updates

:::{note}
Copier will *overwrite* files with the template files. Please check the changes using `git diff` and put back anything you would like to keep from the existing project files.
:::


## If you do not have a skeleton-based project

If you have a project with a different structure then it is best to go straight to the latest release:

```shell
copier copy https://github.com/cmacphillamy/tbioinfo-copier-python.git /path/to/existing-project
git diff
# Examine the changes, put back anything you want to keep
git commit -m "Adopt python-copier-template x.x.x"
```

:::{note}
Copier does not touch any already existing files that do not conflict with the ones in the template. Therefore, you may end up with files in your project you no longer need such as old github workflows. These would need to be manually deleted.
:::
