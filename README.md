# python_env_setup
Codes to set up a Python environment with good coding practices.

## Recommended repos by Andre
- repo: https://github.com/pre-commit/mirrors-mypy
  rev: v0.782
  hooks:
  -   id: mypy
      args: [--ignore-missing-imports, --no-warn-no-return]
- repo: https://github.com/ambv/black
  rev: stable
  hooks:
  -   id: black
- repo: https://github.com/pycqa/flake8
  rev: 3.7.9
  hooks:
      -   id: flake8    