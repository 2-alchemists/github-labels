# 2Alchemists Github Labels

> The way we set up Github labels for our projects at [2Alchemists](https://2alchemists.com).

## Purpose

The default Github labels may be fine for some projects, but we think they can be greatly improved by adding our own labels.

Dave Lunny has written a great [article](https://medium.com/@dave_lunny/sane-github-labels-c5d2e6004b63) about a sane labelling scheme, and this repository takes up most of the ideas in the article, adapting them to our way of working and organizing.

## Format of labels

The labels are specified as JSON files, ready to be used with [popomore/github-labels](https://github.com/popomore/github-labels).

## How to use

See [documentation](https://github.com/popomore/github-labels) for installation and usage of [popomore/github-labels](https://github.com/popomore/github-labels), especially when using a Gitbub Enterprise instance for which you'll need to pass some additional parameters (like a [Personal Access Token](https://github.com/settings/tokens)).

To apply the labels on a specific repository `user/repo`, type the following command:

```sh
$ ls src/*.json | xargs -I{} labels -c {} -f user/repo
```