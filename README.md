# Installation and Usage

1. Install uv:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

2. Create virtual environment and install dependencies:
```bash
uv venv
source .venv/bin/activate  # On Windows, use: .venv\Scripts\activate
uv pip install pre-commit
```

3. Set up pre-commit hooks:
```bash
pre-commit install
```

4. Run pre-commit on all files:
```bash
pre-commit run --all-files
```

### Example Output

If a private key is detected, you'll see output like this:

```
Ethereum secrets detected:
test_file.py:4: Potential Ethereum Private Key detected
```