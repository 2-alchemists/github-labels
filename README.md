# 2Alchemists GitHub Labels

> The way we set up GitHub labels for our projects at [2Alchemists](https://2alchemists.com).

## Purpose

The default GitHub labels may be fine for some projects, but we think they can be greatly improved by adding our own labels.

Dave Lunny has written a great [article](https://medium.com/@dave_lunny/sane-github-labels-c5d2e6004b63) about a sane labelling scheme, and this repository takes up most of the ideas in the article, adapting them to our way of working and organizing.

## Format of labels

The labels are specified as JSON files, ready to be used with [popomore/github-labels](https://github.com/popomore/github-labels).

## Labels

These are the labels already defined.

### Domain

| Name             | Color      |
|------------------|------------|
| `Domain: 🎛 Config` | ![#b56edd](https://via.placeholder.com/15/b56edd/000000?text=+) `#b56edd` |
| `Domain: 👩‍💻 Dev Experience` | ![#18e295](https://via.placeholder.com/15/18e295/000000?text=+) `#18e295` |
| `Domain: 📝 Documentation` | ![#514fe2](https://via.placeholder.com/15/514fe2/000000?text=+) `#514fe2` |
| `Domain: ⚡️ Performance` | ![#f74fdb](https://via.placeholder.com/15/f74fdb/000000?text=+) `#f74fdb` |
| `Domain: 🛡 Security` | ![#0c58d3](https://via.placeholder.com/15/0c58d3/000000?text=+) `#0c58d3` |
| `Domain: 🧪 Testing` | ![#86f411](https://via.placeholder.com/15/86f411/000000?text=+) `#86f411` |
| `Domain: 🛠 Tooling` | ![#fbca04](https://via.placeholder.com/15/fbca04/000000?text=+) `#fbca04` |
| `Domain: 🎨 User Experience` | ![#f4cfb0](https://via.placeholder.com/15/f4cfb0/000000?text=+) `#f4cfb0` |

### Priority

| Name             | Color      |
|------------------|------------|
| `Priority: ⚪️ Low` | ![#009800](https://via.placeholder.com/15/009800/000000?text=+) `#009800` |
| `Priority: 🔵 Medium` | ![#fbca04](https://via.placeholder.com/15/fbca04/000000?text=+) `#fbca04` |
| `Priority: 🔴 High` | ![#d73a4a](https://via.placeholder.com/15/d73a4a/000000?text=+) `#d73a4a` |
| `Priority: 🚨 Critical` | ![#e11d21](https://via.placeholder.com/15/e11d21/000000?text=+) `#e11d21` |

### Type

| Name             | Color      |
|------------------|------------|
| `Type: 🐛 Bug` | ![#e11d21](https://via.placeholder.com/15/e11d21/000000?text=+) `#e11d21` |
| `Type: 🔨 Maintenance` | ![#fbca04](https://via.placeholder.com/15/fbca04/000000?text=+) `#fbca04` |
| `Type: ✨ Enhancement` | ![#84b6eb](https://via.placeholder.com/15/84b6eb/000000?text=+) `#84b6eb` |
| `Type: ❓ Question` | ![#cc317c](https://via.placeholder.com/15/cc317c/000000?text=+) `#cc317c` |

## How to use

See [documentation](https://github.com/popomore/github-labels) for installation and usage of [popomore/github-labels](https://github.com/popomore/github-labels), especially when using a Gitbub Enterprise instance for which you'll need to pass some additional parameters (like a [Personal Access Token](https://github.com/settings/tokens)).

To apply the labels on a specific repository `user/repo`, type the following command:

```sh
$ ls src/*.json | xargs -I{} labels -c {} -f user/repo
```

## Related

- [GitHub API - Labels](https://developer.github.com/v3/issues/labels)
- [popomore/github-labels - Add GitHub labels automatically](https://github.com/popomore/github-labels)
- [Sane GitHub Labels – Dave Lunny – Medium](https://medium.com/@dave_lunny/sane-github-labels-c5d2e6004b63)