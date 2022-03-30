# yeti-python-package

This is a fork of [wemake-services/wemake-python-package](http://github.com/wemake-services/wemake-python-package/), created for my own opinionated personal usage. Changes applied to the original product:

- Sphinx documentation and its helpers removed (because I do not like ReST);
- `flakehell` executed instead of `flake8`, and a custom list of ignores applied.

## Installation

Firstly, you will need to install dependencies:

```bash
pip install cookiecutter jinja2-git lice
```

Then, create the project itself:

```bash
cookiecutter gh:anatoly-scherbakov/yeti-python-package
```

## License

MIT. See [LICENSE](https://github.com/anatoly-scherbakov/yeti-python-package/blob/master/LICENSE) for more details.
