# Project Setup
 
## 1. Install `uv`
 
macOS / Linux:
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```
 
Windows (PowerShell):
```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```
 
Verify:
```bash
uv --version
```
 
## 2. Sync project dependencies
 
From the project root (where `pyproject.toml` / `uv.lock` live):
```bash
uv sync
```

## 3. Run the lab

```bash
uv run jupyter lab
```
`uv run` makes sure the environment is synced before launching, so you don't need to manually activate `.venv` first.
