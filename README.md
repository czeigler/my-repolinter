# my-repolinter

A RepoLinter Docker image to lint my open source projects.

If you want to do the same then just clone the GitHub repo, change the `repolint.json` file in the `src` directory as appropriate and create your own Docker image.

More details can be found at [docker-repolint](https://github.com/markbirbeck/docker-repolinter). If you have any problems or suggestions then please raise them there.

And if you have other best practices that you want to share then please raise them here, through the issue-tracker. Thanks!

## The Ruleset

For a list of *possible* rules, see [Default ruleset](https://github.com/todogroup/repolinter/blob/master/README.md#default-ruleset).

### All languages

These rules are from the base RepoLinter ruleset:
* [license-file-exists](https://github.com/todogroup/repolinter/blob/master/README.md#license-file-exists)
* [readme-file-exists](https://github.com/todogroup/repolinter/blob/master/README.md#readme-file-exists)
* [binaries-not-present](https://github.com/todogroup/repolinter/blob/master/README.md#binaries-not-present)

These rules have been added:
* [editorconfig-file-exists](#editorconfig-file-exists)

#### editorconfig-file-exists

Fails if there isn't a file matching ```.editorconfig``` in the root of the target directory. For details of this file see [EditorConfig](http://editorconfig.org/).
