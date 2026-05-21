# Testing

> Load this file when: writing, running, or debugging tests.

---

## Strategy
_Unit, integration, or end-to-end? What's covered and what's explicitly not._

## Run Tests
```bash
pytest tests/
pytest tests/test_foo.py -v        # single file
pytest -k "test_name" --tb=short   # single test
```

## Test Conventions
- Test files: `tests/test_<module>.py`
- Fixtures in: `tests/conftest.py`
- Mock external calls — never hit live APIs in tests
- Use `output/test_artifacts/` for generated test files (gitignored)

## Coverage
```bash
pytest --cov=src tests/
```

## Known Gaps
_What's not tested and why._
