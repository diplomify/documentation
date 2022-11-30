# MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Install

    pip install -r requirements.txt

## Start Server

    mkdocs serve --dev-addr 127.0.0.1:8001

## Link to Heading IDs

    [Heading IDs](#headingid)

## deploy 

    mkdocs gh-deploy
