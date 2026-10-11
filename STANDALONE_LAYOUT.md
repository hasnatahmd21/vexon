# Standalone ZIP project layout

The canonical standalone copy of `ai_cyber_project.zip` is extracted into `standalone/`.

After extraction, run commands from that directory (the same directory as `run_gates.py`):

```bash
cd standalone
python run_gates.py
python -m unittest discover -s tests -t .
```

The extraction workflow validates archive paths, preserves the package layout (`ai_cyber/`, `ai_cyber/legacy/`, `tests/`, `docs/`, and `tools/`), compiles the project, runs Gates 0–10, and runs complete unittest discovery before committing the extracted files. It does not overwrite the repository's root README or root tests.
