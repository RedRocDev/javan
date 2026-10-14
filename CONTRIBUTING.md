# Contributing to Javan

Thank you for your interest. Javan is presently a **product concept and architecture repository**. Design discussion, requirements, research and feedback are welcome.

## Start here
Read [Vision](docs/VISION.md), [Architecture](docs/ARCHITECTURE.md), [Modules](docs/MODULES.md) and [Roadmap](docs/ROADMAP.md).

## Propose a change
1. Describe the user problem and affected personas.
2. Explain whether the change belongs in Javan Core, an optional Module or Javan Cloud.
3. Include security/privacy implications and cross-platform constraints.
4. Provide a small acceptance test rather than only a screenshot.
5. Avoid assumptions that planning documents equal shipped implementations.

## Planned engineering contribution standards
- Rust formatting, linting and tests; TypeScript type checks and component tests.
- No hardcoded credentials, tokens or personal data.
- Significant dependencies should be justified against startup size, portability and update costs.
- All modules must declare capabilities, supported platforms, upgrades and removal behaviour.
- Security-sensitive changes need review and regression coverage.

## Licensing
No open-source licence has been selected yet. **A public repository is not automatically open-source licensed.** Until a licence is added, please don't assume reuse, distribution or modification rights beyond those GitHub provides by default. Contributors should seek maintainer guidance before contributing substantial code.

## Product / brand
Javan is the product; Open Javan Labs and RedRoc Dev are its associated brand identities.
