SHELL:=/usr/bin/env bash

.PHONY: lint
lint:
	poetry run mypy {{ cookiecutter.project_name.lower().replace('-', '_') }} tests
	poetry run flakehell lint {{ cookiecutter.project_name.lower().replace('-', '_') }} tests

.PHONY: unit
unit:
	poetry run pytest

.PHONY: package
package:
	poetry check
	poetry run pip check
	poetry run safety check --full-report

.PHONY: test
test: lint package unit

