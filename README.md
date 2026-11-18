# Sisdeve Agro

Sisdeve Agro is a modular monolith designed for grain farm management.

## Project status

The project is in its initial backend setup stage. Business modules and
persistent storage will be introduced incrementally.

## Repository structure

- `back/`: Go backend, developer automation, and future API modules.
- `infra/`: Infrastructure configuration (to be added when required).
- `front/`: React frontend (planned after the backend MVP).

## Requirements

- Go 1.27.4
- Git
- GNU Make

## Getting started

From the repository root:

```bash
make -C back run
make -C back test
make -C back build
```

## Engineering principles

- Modular monolith with explicit module boundaries.
- Domain rules independent of database drivers.
- Test-driven development for business behavior.
- Contextual commits and Git Flow using `main` and `develop`.

## Language

Source code and technical identifiers use English. User-facing messages
are written in Brazilian Portuguese.

For the Portuguese guide, see [README_pt-br.md](README_pt-br.md).