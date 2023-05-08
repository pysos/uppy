<p align="center">
  <a href="https://github.com/pysos/uppy"><img alt="uppy" src="https://raw.githubusercontent.com/pysos/uppy/main/logo/uppy-logo-with-text.svg" width="60%"></a>
  <p align="center">Command-line updater for all project dependencies.</p>
</p>

[![PyPi Version](https://img.shields.io/pypi/v/uppy.svg?style=flat-square)](https://pypi.org/project/uppy/)

uppy is a command-line tool that updates all of your project dependencies.
Handles dependencies from

- package.json
- GitHub actions
- pre-commit

Usage with example output:

```
uppy /path/to/project
```

```
.pre-commit-config.yaml:

  https://github.com/charliermarsh/ruff-pre-commit   v0.0.231   ❯   v0.0.265
  https://github.com/psf/black                       22.12.0    ❯   23.3.0
  https://github.com/pre-commit/mirrors-prettier     v2.7.0     ❯   v2.7.1

.github/workflows/tests.yml:

  actions/checkout                     v3
  pre-commit/action                    v3.0.0
  actions/checkout                     v3
  actions/setup-python                 v4
  actions/setup-python                 v4
  nschloe/action-cached-lfs-checkout   v1

.github/workflows/release.yml:

  nschloe/action-cached-lfs-checkout     v1
  actions/setup-python                   v4
  pypa/gh-action-pypi-publish            release/v1
  actions/checkout                       v3
  actions/setup-python                   v4
  JamesIves/github-pages-deploy-action   v4
  actions/checkout                       v3
  JamesIves/github-pages-deploy-action   v4

Update? [Y/n]
```

### Installation

Install uppy [from PyPI](https://pypi.org/project/uppy/) with

```
pip install uppy
```

### How to get a license

Licenses for personal and academic use can be purchased
[here](https://buy.stripe.com/cN2aHngZE1IC3iEeV0).
You'll receive a confirmation email with a license key.
Install the key with

```
plm add <your-license-key>
```

on your machine and you're good to go.

For commerical use, please contact support@mondaytech.com.
