
# Agent-0.1
A modern Python project setup using:
- [`tox`](https://tox.readthedocs.io/) – for test, lint, and format automation
- [`uv`](https://github.com/astral-sh/uv) – for fast dependency installation and environment management
- [`ruff`](https://docs.astral.sh/ruff/) – for linting and formatting
- [`pre-commit`](https://pre-commit.com/) – to automatically run checks before every commit (optional)
---

## 🧪 Run Tasks with Tox
### ✅ Run tests
```bash
tox -e test
```

### 🔍 Run Ruff linter
```bash
tox -e lint
```

### 🎨 Check formatting with Ruff
```bash
tox -e format
```
---

## 💡 Manual Ruff Usage
If you want to run Ruff directly:

### Format the code
```bash
ruff format .
```

### Check for lint issues
```bash
ruff check .
```
---

## 🔄 Pre-commit Hook Setup (Optional)

Enable automatic checks before every commit:
```bash
pre-commit install
```

> Every time you commit, Ruff will check lint and formatting.
> If any checks fail, the commit is blocked until issues are resolved.

To manually run the hooks (e.g. after cloning):
```bash
pre-commit run --all-files
```
---

## 📁 Project Structure
```
agent-0.1/
├── tests/                  # Tests
├── requirements-agent.txt  # Agent dependencies
├── requirements-test.txt   # Test dependencies
├── tox.ini                 # Tox environment definitions
├── pyproject.toml          # Tool configurations (ruff, etc)
└── README.md               # Project documentation
```
---

## ✅ Add More Tox Environments
You can expand the `tox.ini` file to include:
- Integration or end to end test suites

Tox will help you organize and automate it all.
---

## 🧊 Using UV
This project uses [`uv`](https://github.com/astral-sh/uv) for:
- Creating fast virtual environments (`uv venv`)
- Installing packages (`uv pip install`)
- Installing dependencies in Tox (`installer = uv`)
---

## 🔗 Useful Links
- [Tox Documentation](https://tox.readthedocs.io/)
- [Ruff Documentation](https://docs.astral.sh/ruff/)
- [Pre-commit Hooks](https://pre-commit.com/)
- [UV Project](https://github.com/astral-sh/uv)
---

Happy hacking 🎉
