

# qboot 🚀

**qboot** is a modern, lightning-fast command-line tool designed to bootstrap a complete and professional Python project in seconds. It eliminates the boilerplate setup, allowing you to focus on what truly matters: your code.

With a single command, `qboot` generates a feature-rich project structure, complete with a virtual environment, best-practice development tools, and pre-configured settings for linting, formatting, and testing.

---

## ✨ Features

- **Cross-Platform:** Works seamlessly on Windows, macOS, and Linux.
- **Virtual Environment:** Automatically creates a `.venv` virtual environment to isolate project dependencies.
- **Modern Tooling:** Installs and configures a suite of essential development tools out-of-the-box:
  - **Formatting:** `black`, `ruff-format`
  - **Linting:** `ruff`
  - **Import Sorting:** `isort`
  - **Type Checking:** `mypy`
  - **Testing:** `pytest`
  - **Dependency Management:** `pip-tools`
  - **Git Hooks:** `pre-commit`
- **Sensible Defaults:** Generates configuration files with community-accepted best practices:
  - `pyproject.toml` (PEP 621 compliant)
  - `.pre-commit-config.yaml`
  - `mypy.ini`
  - `.gitignore`
  - `.editorconfig`
- **IDE-Friendly:** Includes a `.vscode/settings.json` file with recommended settings for Visual Studio Code.
- **Git Integration:** Initializes a new Git repository and creates the first commit, so you're ready for version control from day one.

---

## 📦 Installation

You can install `qboot` directly from PyPI:

```bash
pip install qboot
````

---

## 🚀 Quick Start

Getting started is as simple as running one command.

**Create a new project:**

```bash
qboot my-awesome-project
```

**Navigate into your new project and activate the virtual environment:**

```bash
cd my-awesome-project
```

**On macOS/Linux:**

```bash
source .venv/bin/activate
```

**On Windows:**

```bash
.venv\Scripts\activate
```

**Run the initial tests to verify the setup:**

```bash
pytest
```

That's it! You now have a fully configured, production-ready Python project.

---

## ⚙️ Command-Line Options

`qboot` provides several options to customize the project setup.

| Option            | Description                                           | Default              |
| ----------------- | ----------------------------------------------------- | -------------------- |
| `project_name`    | The name of the project/package to create. (Required) | -                    |
| `--python <path>` | Path to the Python executable for the venv.           | The current `python` |
| `--dir <path>`    | Target directory to create the project in.            | `./<project_name>`   |
| `--no-mypy`       | Skip the setup for `mypy`.                            | Enabled              |
| `--no-precommit`  | Skip `pre-commit` setup and hook installation.        | Enabled              |
| `--no-piptools`   | Skip `pip-tools` and requirements compilation.        | Enabled              |

**Example:**

```bash
# Create a project named 'api-service' without mypy support
qboot api-service --no-mypy
```

---

## 🌱 Contributing

Contributions are welcome and greatly appreciated!
Whether it's reporting a bug, proposing a new feature, or improving the documentation, your help makes `qboot` better for everyone.

To contribute, please follow these steps:

1. Fork the repository on GitHub.
2. Clone your fork to your local machine.
3. Create a new branch for your changes.
4. Make your changes and commit them with a clear, descriptive message.
5. Push your branch to your fork on GitHub.
6. Open a pull request to the main `qboot` repository.

---

## 📜 License

This project is licensed under the MIT License.
See the [LICENSE](LICENSE) file for more details.





