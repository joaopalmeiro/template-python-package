# Template Notes

- https://github.com/joaopalmeiro/template-python-cli
- Hatch:
  - https://hatch.pypa.io/1.9/config/build/#packages
  - https://pypi.org/project/hatch/
  - https://hatch.pypa.io/dev/history/hatch/
  - https://github.com/ofek/pyapp
  - https://hatch.pypa.io/dev/config/internal/testing/
  - https://hatch.pypa.io/dev/config/environment/overview/#type
  - https://hatch.pypa.io/dev/plugins/environment/virtual/
  - https://hatch.pypa.io/dev/blog/2024/05/02/hatch-v1100/#uv
  - https://hatch.pypa.io/dev/how-to/environment/select-installer/
  - `installer = "uv"` or `installer = "pip"`
  - https://hatch.pypa.io/latest/config/build/#output-directory
- https://www.pythonpapers.com/p/how-to-publish-a-python-package-to
- https://dev.to/astrojuanlu/python-packaging-is-great-now-uv-is-all-you-need-4i2d
- mypy:
  - https://pypi.org/project/mypy/
  - https://github.com/python/mypy/blob/master/CHANGELOG.md
  - https://github.com/pydantic/pydantic/blob/v2.6.3/docs/integrations/mypy.md#configuring-the-plugin
  - https://github.com/FlorianWilhelm/the-hatchlor/blob/v0.3/%7B%7Bcookiecutter.project_slug%7D%7D/pyproject.toml#L81
  - https://peps.python.org/pep-0742/:
    - "Narrowing types with TypeIs"
    - https://github.com/python/mypy/blob/v1.11.1/CHANGELOG.md#support-typeis-pep-742
    - "`TypeIs` will be added to the `typing` module in Python 3.13 (...)"
  - https://github.com/python/mypy/blob/v1.11.1/CHANGELOG.md#support-for-functoolspartial: "Mypy now type checks uses of `functools.partial`. Previously mypy would accept arbitrary arguments."
  - https://github.com/python/mypy/blob/v1.11.1/CHANGELOG.md#stricter-checks-for-untyped-overrides: "Past mypy versions didn't check if untyped methods were compatible with overridden methods. This would result in false negatives. Now mypy performs these checks when using `--check-untyped-defs`."

## Commands

```bash
hatch new --interactive hatch-demo
```

```bash
hatch env show --internal
```

```bash
hatch env show --json
```
