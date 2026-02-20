# Trunk Docs

This repository contains the documentation site for [Trunk](https://trunk.io), powered by [Fern](https://buildwithfern.com).

## Repository Structure

```
fern/
├── fern.config.json          # Fern project configuration
├── docs.yml                  # Documentation site layout, navigation, and styling
├── apis/
│   ├── flaky-tests-api/
│   │   ├── openapi.yml       # Flaky Tests API spec
│   │   └── generators.yml    # Generator config
│   └── merge-queue-api/
│       ├── openapi.yml       # Merge Queue API spec
│       └── generators.yml    # Generator config
└── docs/
    ├── assets/               # Logos and favicon
    └── pages/                # Documentation content (MDX)
        ├── merge-queue/
        ├── flaky-tests/
        ├── ci-autopilot/
        ├── code-quality/
        └── setup/
```

## Prerequisites

Install the Fern CLI:

```bash
npm install -g fern-api
```

## Development

Preview the docs locally:

```bash
fern docs dev
```

This starts a local development server so you can see changes in real time.

## Generating the Docs

To generate and publish the documentation site:

```bash
fern generate --docs
```

## Editing Content

- **Pages** are written in MDX and live in `fern/docs/pages/`.
- **Navigation and layout** are configured in `fern/docs.yml`.
- **API references** are auto-generated from the OpenAPI specs in `fern/apis/`.

## Useful Links

- [Fern Documentation](https://docs.buildwithfern.com)
- [Trunk Dashboard](https://app.trunk.io)
