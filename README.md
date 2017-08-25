# Github-clone

## Description

Github-clone makes it easy to clone all github projects of a user, using either the public or private clone urls for the projects.

## Examples

Clone all repositories of user Narnach, using the public clone URLs:

    github-clone Narnach
  
Clone all repositories of user Narnach, using the private clone URLs and suppressing console output:

    github-clone Narnach -q --private

## Configuration

You can use the 

## Ideas / todo

* Add support to fetch/pull repositories as well as clone them. This makes automatic backups a possibility.
* Turn this script into a proper ruby gem.
* Add support to clone gitosis-managed repositories.

## Author

Copyright (c) 2008-2017 - Wes Oldenbeuving, released under the MIT license.