# Github-clone

## Description

Github-clone makes it easy to clone all github projects of a user, using either the public or private clone urls for the projects.
This version adds option modified to clone to bare repository with "--mirror"

## Examples

Clone all public repositories of user Narnach, using the public clone URLs:

    github-clone Narnach
  
Clone all repositories of user Narnach, using the private clone URLs and suppressing console output:

    github-clone Narnach -q --private

When you simply want a list of your repositories with their clone urls, that's an option too:

    github-clone Narnach --dry-run --private

The output will look something like this:

    Username matches github.user configuration, so using that to access private repositories.
    Would clone aasterinian: git@github.com:Govannon/aasterinian.git
    Would clone future: git@github.com:Narnach/future.git
    Already exists: github-clone for git@github.com:Narnach/github-clone.git

As you can see this accounts for your private organizations and collaborator repos as well.

## Configuration
    
When you have your `github.user` and `github.token` properly setup ([howto]( https://github.com/blog/180-local-github-config )) in your `~/.gitconfig`, `github-clone` will use that information to fetch a list of your private repositories and clone those in addition to your public repositories.

You can find and/or setup your access tokens here. You only need the `repo` scope:  [https://github.com/settings/tokens]()

## Ideas / todo

* Add support to fetch/pull repositories as well as clone them. This makes automatic backups a possibility.
* Turn this script into a proper ruby gem.
* Add support to clone gitosis-managed repositories.

## Author

Copyright (c) 2008-2017 - Wes Oldenbeuving, released under the MIT license.