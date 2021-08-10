# python_env_setup
Codes to set up a Python environment with good coding practices.
---

Instructions [ref](https://pre-commit.com/)

- Create virtual environment: `python3 -m venv venv`

- Enter virutal environment: `source venv/bin/activate`

- Install pre-commit: `pip install pre-commit`

- Freeze requirements: `pip freeze > requirements.txt`

- Set up custom git log format: [[ref]](https://stackoverflow.com/questions/1838873/visualizing-branch-topology-in-git/34467298#34467298)
	- Add to .gitconfig:
		```
		[alias]
			lg = lg1
			lg1 = lg1-specific --all
			lg2 = lg2-specific --all
			lg3 = lg3-specific --all

			lg1-specific = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(auto)%d%C(reset)'
			lg2-specific = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(auto)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)'
			lg3-specific = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset) %C(bold cyan)(committed: %cD)%C(reset) %C(auto)%d%C(reset)%n''          %C(white)%s%C(reset)%n''          %C(dim white)- %an <%ae> %C(reset) %C(dim white)(committer: %cn <%ce>)%C(reset)'
		```


# Tips from Andre
pytest-testmon
pytest-cov
black

[pre-commit-hooks](https://github.com/pre-commit/pre-commit-hooks)


python conventional commits
python semantic versioning
changelog.md


# Design Patterns - References
- [Design Patterns](https://sourcemaking.com/design_patterns)
