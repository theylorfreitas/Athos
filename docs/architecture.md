# Architecture

Athos is organized around a small set of core layers:

- memory: operational context stored in `_memoria/`
- identity: visual and voice guidance in `identidade/`
- skills: specialized workflows in `.claude/skills/`
- documentation: public-facing guidance in `docs/`

This separation keeps the system modular and easy to extend.
