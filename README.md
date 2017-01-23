# OCaml esy project

[![Build Status](https://travis-ci.org/andreypopp/esy-ocaml-project.svg?branch=master)](https://travis-ci.org/andreypopp/esy-ocaml-project)

A project which demonstrates an OCaml workflow with esy.

## Installation

You need to install esy first:

    % npm install -g @andreypopp/esy

Then just use `esy install` as usual:

    % esy install

## Build

    % esy build

## Clean build artifcats

    % esy clean

## Shell into build environment

    % esy shell

## Run preconfigured OCaml REPL

    % esy repl

## Merlin

Merlin integration is included. If your editor of choice has Merlin
plugin/extension then you can run execute it like this:

    % esy vim ./bin/hello.ml

## Merlin + Vim

Merlin ships with Vim plugin, to enable it add the following lines to `.vimrc`:

    if $opam_merlin__install != ''
      execute "set rtp+=" . $opam_merlin__install . "/share/merlin/vim"
    endif
