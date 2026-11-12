# Open Glass Suite

**Open Glass Suite (OGS)** is a growing collection of visual customizations and utilities designed to give existing software a consistent, minimalist glass-style interface.

The guiding idea is simple: **extend existing software where possible; replace it only when necessary.**

OGS is an independent, experimental project. It is being developed incrementally, with Windows as the initial target.

> **Project status:** Early planning and proof-of-concept. There are no public application releases yet.

## Principles

- **Extension-first.** Prefer extensions, add-ons, plugins, and themes that preserve the original application's features, updates, accounts, and sync.
- **Real transparency where feasible.** Aim for actual desktop/window transparency and carefully controlled blur, not just translucent colors within a webpage.
- **Minimal and readable.** Dark surfaces, subtle borders, restrained animation, clear contrast, and configurable opacity.
- **Native when needed.** Use small OS-native helpers for capabilities that an extension cannot provide; avoid replacing a whole application for a visual modification.
- **Lean and independent.** Keep resource use and background activity modest. Each component should work without requiring the rest of the suite.
- **Reversible and maintainable.** Prefer opt-in changes, straightforward rollback, and compatibility with upstream updates.

These are project goals, not claims that every effect will work in every application or environment.

## First experiment: Open Glass Browser

The first planned component will explore making **Google Chrome's webpages visually transparent to the Windows desktop**, while retaining Chrome itself.

The proposed route is a Chrome extension for webpage styling, with an optional small Windows-native helper if the browser cannot provide true desktop transparency on its own.

The initial work will test technical feasibility, particularly Chrome's rendering and Windows composition behavior. The approach may change based on those results. It is **not currently a standalone browser fork**, and no universal website compatibility is promised.

See the [roadmap](docs/ROADMAP.md) for the current scope.

## Projects and releases

Individual components are developed in separate private repositories while they are experimental. This public repository is intended to hold the **documentation, curated source snapshots, and downloadable releases** of components when they are ready to publish.

Each component will have its own version and release notes. Publishing one component should not require rebuilding or releasing the others.

The planned public structure and release process are described in [Repository and Releases](docs/REPOSITORY_AND_RELEASES.md).

**There are no installers, browser extensions, or release builds available here yet.** When published, they will appear in the relevant project directories and the repository's GitHub Releases.

## Documentation

- [Project vision and design principles](docs/VISION.md)
- [Development roadmap](docs/ROADMAP.md)
- [Repository structure and release process](docs/REPOSITORY_AND_RELEASES.md)

## Licensing and contributions

A software license has **not yet been selected**. Public access to this repository does not, by itself, grant permission to redistribute or modify its contents. A license will be added before publishing reusable project source code.

Feedback and ideas are welcome through GitHub Issues. Development repositories are currently private, so the public repository is not yet set up as the primary place for code contributions.
