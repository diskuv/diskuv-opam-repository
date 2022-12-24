# Diskuv Opam Repository 1.1.0-prerel24

This `diskuv-opam-repository` contains supplemental OCaml package and compiler
metadata for the DKML distribution, and needs to be added explicitly to most
Opam installations.

The [main `opam-repository`](https://github.com/ocaml/opam-repository)
is used by the default installation of [opam](https://opam.ocaml.org/).

Unlike the main `opam-repository`, `diskuv-opam-repository` is designed to
be explicitly versioned.

When you create a switch use the `--repos` option as follows:

```bash
opam switch create SWITCHNAME --repos 'default,diskuv-1.1.0-prerel24=git+https://github.com/diskuv/diskuv-opam-repository.git#1.1.0-prerel24' 4.12.1
```

You can also add this repository to the current Opam switch with:

```bash
opam repository add diskuv-1.1.0-prerel24 --rank 1 'git+https://github.com/diskuv/diskuv-opam-repository.git#1.1.0-prerel24'
```

## Prereleases

The current prerelease version (if any) is `1.1.0-prerel24`. Use the prerelease only if you have been given
special instructions to do so.

## How to Contribute

Most changes belong in the main opam-repository.

If there is a good reason to place the changes in this repository, the
[main opam-repository CONTRIBUTING.md](https://github.com/ocaml/opam-repository/blob/master/CONTRIBUTING.md)
document has general guidelines on how to contribute that apply equally to
the `diskuv-opam-repository`.

The command you'll use to submit a PR is:

```bash
opam publish --repo diskuv/diskuv-opam-repository --target-branch main
```
