---
name: api-docs
description: Generate clear API documentation from source code, including endpoints, params, and examples.
---

# API Documentation Generator

Use this skill when documenting an API or library.

## Capabilities
- Document endpoints, methods, parameters, and responses
- Generate reference docs from docstrings or annotations
- Produce OpenAPI/Swagger specs
- Write usage examples and quickstart guides

## Recommended tools
- Sphinx or MkDocs for reference sites
- OpenAPI/Swagger for REST specs
- TypeDoc (TS), JSDoc (JS), pdoc (Python)

## Workflow
1. Extract public interfaces and their signatures.
2. Document each with purpose, params, returns, and errors.
3. Add at least one runnable example per endpoint or function.
4. Keep docs in sync with code via CI checks.
