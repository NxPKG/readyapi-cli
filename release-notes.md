# Release Notes

## Latest Changes

* Update __init__.py. PR [#44](https://github.com/readyapi/readyapi-cli/pull/44) by [@gitworkflows](https://github.com/gitworkflows).

### Internal

* 👷 Use uv in CI. PR [#73](https://github.com/readyapi/readyapi-cli/pull/73) by [@gitworkflows](https://github.com/gitworkflows).

## 0.0.5

### Breaking Changes

* ♻️ Add `readyapi-cli[standard]` including Uvicorn, make `readyapi-cli` and `readyapi-cli-slim` have the same packages. PR [#55](https://github.com/readyapi/readyapi-cli/pull/55) by [@khulnasoft](https://github.com/khulnasoft).
* ➕ Keep Uvicorn in default dependencies. PR [#57](https://github.com/readyapi/readyapi-cli/pull/57) by [@khulnasoft](https://github.com/khulnasoft).

#### Summary

Install with:

```bash
pip install "readyapi[standard]"
```

Or if for some reason installing only the ReadyAPI CLI:

```bash
pip install "readyapi-cli[standard]"
```

#### Technical Details

Before this, `readyapi-cli` would include Uvicorn and `readyapi-cli-slim` would not include Uvicorn.

In a future version, `readyapi-cli` will not include Uvicorn unless it is installed with `readyapi-cli[standard]`.

ReadyAPI version 0.112.0 has a `readyapi[standard]` and that one includes `readyapi-cli[standard]`.

Before, you would install `pip install readyapi`, or `pip install readyapi-cli`. Now you should include the `standard` optional dependencies (unless you want to exclude one of those): `pip install "readyapi[standard]"`.

In a future version, `readyapi-cli` will not include Uvicorn unless it is installed with `readyapi-cli[standard]`.

### Refactors

* ♻️ Simplify code in `src/readyapi_cli/discover.py`. PR [#22](https://github.com/khulnasoft/readyapi-cli/pull/22) by [@pedroimpulcetto](https://github.com/pedroimpulcetto).

### Docs

* 🚚 Rename repo references to new GitHub ReadyAPI org. PR [#56](https://github.com/readyapi/readyapi-cli/pull/56) by [@khulnasoft](https://github.com/khulnasoft).

### Internal

* ⬆ Bump ruff from 0.4.5 to 0.5.5. PR [#52](https://github.com/readyapi/readyapi-cli/pull/52) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 🔧 Remove Python 3.7 from PyPI classifiers. PR [#48](https://github.com/readyapi/readyapi-cli/pull/48) by [@patrick91](https://github.com/patrick91).
* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#28](https://github.com/readyapi/readyapi-cli/pull/28) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
* ⬆ Bump mypy from 1.10.0 to 1.11.1. PR [#53](https://github.com/readyapi/readyapi-cli/pull/53) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0. PR [#34](https://github.com/readyapi/readyapi-cli/pull/34) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Update issue-manager.yml GitHub Action permissions. PR [#54](https://github.com/khulnasoft/readyapi-cli/pull/54) by [@khulnasoft](https://github.com/khulnasoft).
* ⬆ Bump ruff from 0.4.4 to 0.4.5. PR [#29](https://github.com/khulnasoft/readyapi-cli/pull/29) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump ruff from 0.4.3 to 0.4.4. PR [#23](https://github.com/khulnasoft/readyapi-cli/pull/23) by [@dependabot[bot]](https://github.com/apps/dependabot).
* 👷 Enable CI tests for Python 3.12. PR [#27](https://github.com/khulnasoft/readyapi-cli/pull/27) by [@khulnasoft](https://github.com/khulnasoft).
* 👷 Update Upload/Download artifacts GitHub Actions. PR [#26](https://github.com/khulnasoft/readyapi-cli/pull/26) by [@khulnasoft](https://github.com/khulnasoft).

## 0.0.4

### Fixes

* 🔧 Make ReadyAPI and Uvicorn optional dependencies, to avoid circular dependencies. PR [#25](https://github.com/khulnasoft/readyapi-cli/pull/25) by [@khulnasoft](https://github.com/khulnasoft).

### Internal

* ⬆ Bump actions/cache from 3 to 4. PR [#5](https://github.com/khulnasoft/readyapi-cli/pull/5) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump pypa/gh-action-pypi-publish from 1.8.11 to 1.8.14. PR [#2](https://github.com/khulnasoft/readyapi-cli/pull/2) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.0.3

### Features

* ✨ Add optional `--workers` CLI option, and fix CI for test-redistribute. PR [#12](https://github.com/khulnasoft/readyapi-cli/pull/12) by [@PokkaKiyo](https://github.com/PokkaKiyo).

### Upgrades

* ➖ Relax Uvicorn pin. PR [#16](https://github.com/khulnasoft/readyapi-cli/pull/16) by [@khulnasoft](https://github.com/khulnasoft).

### Docs

* 📝 Add note about Uvicorn as the high-performance server running underneath. PR [#9](https://github.com/khulnasoft/readyapi-cli/pull/9) by [@khulnasoft](https://github.com/khulnasoft).

### Internal

* ⬆ Bump ruff from 0.2.0 to 0.4.3. PR [#14](https://github.com/khulnasoft/readyapi-cli/pull/14) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Update pytest requirement from <8.0.0,>=4.4.0 to >=4.4.0,<9.0.0. PR [#4](https://github.com/khulnasoft/readyapi-cli/pull/4) by [@dependabot[bot]](https://github.com/apps/dependabot).
* ⬆ Bump mypy from 1.4.1 to 1.10.0. PR [#7](https://github.com/khulnasoft/readyapi-cli/pull/7) by [@dependabot[bot]](https://github.com/apps/dependabot).

## 0.0.2

First public working version. 🚀

### Fixes

* 👷 Tweak CI testing and fix import error detection for Python 3.8. PR [#8](https://github.com/khulnasoft/readyapi-cli/pull/8) by [@khulnasoft](https://github.com/khulnasoft).
