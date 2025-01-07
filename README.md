<div align="center">
  <img src="https://github.com/kairos-xx/GitPyPi_3.12/raw/main/assets/icon_raster.png" alt="Replit Info API Logo" width="150"/>
  <h1>Python Project Template with GitHub and PyPI Integration</h1>
  <p><em>This template provides a complete setup for Python projects with automated GitHub repository creation and PyPI package publishing capabilities.</em></p>

  <a href="https://replit.com/@kairos/GitPyPi312">
    <img src="https://github.com/kairos-xx/GitPyPi_3.12/raw/main/assets/replit.png" alt="Try it on Replit" width="150"/>
  </a>
</div>
# Python Project Template with GitHub and PyPI Integration

This template provides a complete setup for Python projects with automated GitHub repository creation and PyPI package publishing capabilities.

## Key Features

- Automated GitHub repository setup
- PyPI package publishing workflow
- Code formatting with Black, Ruff, and isort
- Code quality checks with Flake8 and Pyright
- Test coverage with Pytest
- Project archiving functionality
- Comprehensive workflow automation

## Core Scripts

### prepare_environment.py

The main setup script that:
1. Configures project structure
2. Sets up GitHub repository
3. Installs dependencies
4. Creates necessary configuration files

Key components of the script:
- Package management functions
- GitHub repository setup
- Project file generation
- Version control initialization

### Configuration Dictionary Structure

The script uses a comprehensive `project_info` dictionary that contains:

```python
project_info = {
    "templates": {
        # File templates for pyproject.toml, setup.py, etc.
    },
    "classifiers": {
        # PyPI project classifiers
    },
    "setup": {
        "paths": {
            # Project file paths configuration
        },
        "classifiers": {
            # Project-specific classifiers
        },
        "version": "0.1.1",
        "description": "",
        "user_config": {
            # User information
        },
        "urls": {
            # Project URLs
        },
        "requirements": [
            # Project dependencies
        ],
        "nix_packages": [
            # Nix environment packages
        ],
        "required_packages": [
            # Essential packages for setup
        ]
    }
}
```

### Other Utility Scripts

- **pypi_upload.py**: Handles PyPI package versioning and publishing
- **create_zip.py**: Creates project archives

## Getting Started

1. Ensure environment variables are set:
   - GITHUB_TOKEN
   - REPLIT_TOKEN
   - PYPI_TOKEN (for publishing)

2. Run the prepare environment script:
   ```bash
   python scripts/prepare_environment.py
   ```

3. Use the Tools menu in Replit to run workflows for:
   - Code formatting
   - Testing
   - Package publishing
   - Project archiving

## Project Structure

```
├── scripts/          # Utility scripts
├── src/             # Source code
├── tests/           # Test files
├── logs/            # Log outputs
├── zip/             # Archive storage
└── assets/          # Project assets
```
