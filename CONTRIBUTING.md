# Contributing to ManganeseAI

Thank you for helping improve ManganeseAI. Contributions in materials science, computational chemistry, crystallography, electrochemistry, machine learning, and scientific software are welcome.

## Ways to Contribute

- Report bugs, unclear documentation, or reproducibility issues through GitHub Issues.
- Propose features or scientific workflows before starting substantial implementation.
- Submit focused pull requests with tests and documentation where appropriate.
- Improve data validation, provenance, and explanations of scientific assumptions.

For substantial changes, open an issue first to discuss the scope and approach.

## Development Setup

ManganeseAI targets Python 3.11 and uses `uv` for reproducible environments. Clone the repository, open its root directory, then install the locked development dependencies:

```bash
uv sync --locked --extra dev
```

Run the test suite before submitting changes:

```bash
uv run --locked pytest
```

The database defaults to `database/manganeseai.db`. Set `MANGANESEAI_DATABASE_URL` to use another SQLAlchemy database URL. Database initialization is repeatable and does not remove existing records; use a disposable database when testing workflows that write data.

## Scientific Data and Reproducibility

Scientific integrity is central to this project:

- Preserve the original source and database identifier for imported records, along with retrieval details and measurement conditions when available.
- Keep experimental measurements distinct from computationally predicted properties.
- Record units and document transformations, assumptions, and data-processing steps.
- Do not invent, infer, or silently impute measurements. Represent missing values explicitly and document any imputation method used for analysis.
- Do not describe a prediction or candidate ranking as experimentally verified without supporting experimental evidence.
- Keep collection scope and limits explicit. Do not ingest proposed batches or modify production data without the relevant review and approval.

## Credentials and Generated Data

Never commit API keys, tokens, passwords, or other credentials. Use environment variables or Codespaces secrets for credentials such as `MP_API_KEY`; do not place secrets in source code, notebooks, configuration files, logs, or issue comments.

Do not commit generated source snapshots or database files unless a change explicitly requires a reviewed, reproducible fixture. Keep test and exploratory collection runs small, and use dry-run options when available.

## Pull Requests

Keep each pull request focused and explain:

- What changed and why.
- Any scientific assumptions, data sources, schema changes, or compatibility impact.
- How the change was tested, including commands and any tests that could not be run.

Before opening a pull request:

- Run the relevant tests; run the full suite with `uv run --locked pytest` when practical.
- Update documentation and configuration examples affected by the change.
- Check that no secrets, local databases, or unintended generated data are included.
- For data-related changes, verify source attribution, units, provenance, and the distinction between experimental and computational records.

Use a clear pull request title and link the related issue when applicable. Be constructive and specific in reviews and discussions.

## License

By contributing, you agree that your contributions will be made available under the repository's MIT License.
