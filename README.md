# template-python-package

[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
[![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)

Opinionated Python template for new packages.

- [Source code](https://github.com/joaopalmeiro/template-python-package)
- [PyPI package](https://pypi.org/project/template-python-package/)
- [Snyk Advisor](https://snyk.io/advisor/python/template-python-package)

## Getting Started

1. Go to or create the package folder.
2. Get the template files:

```bash
npx degit github:joaopalmeiro/template-python-package
```

or

```bash
npx degit github:joaopalmeiro/template-python-package --force
```

3. Search for `template-python-package` and replace it with the package name. Ignore the template repository URL in the [NOTES.md](NOTES.md) file.
4. Search for `template_python_package` and replace it with the underscored version of the package name.
5. Search for `Opinionated Python template for new packages.` and replace it with the (short) package description.
6. Search for `João Palmeiro` and replace it with the author's name.
7. Search for `joaopalmeiro@proton.me` and replace it with the author's email address.
8. Open the [pyproject.toml](pyproject.toml) file and add the package-specific dependencies. See the [`Dependency configuration`](https://hatch.pypa.io/latest/config/dependency/) and [`Environment configuration`](https://hatch.pypa.io/latest/config/environment/overview/#dependencies) pages in the Hatch documentation for more information (if necessary).
9. Update the `Source code` link at the top to the package repository link (if necessary).
10. Change `GitHub` in the [`Deployment`](#deployment) section to `GitLab` or `Codeberg` and update the link to the corresponding Tags page (if necessary).
11. Update the `Issues` and `Source` fields in the [pyproject.toml](pyproject.toml) file with their respective repository-related links (if necessary).
12. Remove `hatch-demo/` from the [.gitignore](.gitignore) file.
13. Delete the [TEMPLATE.md](TEMPLATE.md) file.
14. Delete the [`Getting Started`](#getting-started) section.

## Development

Install [pyenv](https://github.com/pyenv/pyenv) (if necessary).

```bash
pyenv install && pyenv versions
```

```bash
pip install hatch==1.12.0 && hatch --version
```

```bash
hatch config set dirs.env.virtual .hatch
```

```bash
hatch config show
```

```bash
hatch env create
```

```bash
hatch status
```

```bash
hatch env show
```

```bash
hatch dep show table
```

```bash
hatch run qa:lint
```

```bash
hatch run qa:format
```

```bash
hatch project metadata
```

## Deployment

```bash
hatch version micro
```

```bash
hatch version minor
```

```bash
hatch version major
```

```bash
hatch build --clean
```

```bash
echo "v$(hatch version)" | pbcopy
```

- Commit and push changes.
- Create a tag on [GitHub Desktop](https://github.blog/2020-05-12-create-and-push-tags-in-the-latest-github-desktop-2-5-release/).
- Check [GitHub](https://github.com/joaopalmeiro/template-python-package/tags).

```bash
hatch publish
```

- Check [PyPI](https://pypi.org/project/template-python-package/).
