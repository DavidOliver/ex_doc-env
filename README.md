# ExDoc env

A [Devbox](https://www.jetpack.io/devbox/) environment for [ExDoc](https://hexdocs.pm/ex_doc/readme.html).

## Setup

ExDoc is added as a Git submodule. To checkout the submodule when cloning:

    $ git clone --recurse-submodules git@github.com:DavidOliver/ex_doc-env.git

You can subsequently add your own fork of ExDoc as a remote from within the `ex_doc` directory.

    $ cd ex_doc
    $ git remote add <name> <url>

## Usage

Launch the environment:

    $ devbox shell

Develop ExDoc as usual:

    (devbox) $ cd ex_doc
    (devbox) $ mix setup
    (devbox) $ mix build
    (devbox) $ npm run --prefix assets build:watch
