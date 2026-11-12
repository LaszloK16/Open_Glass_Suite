# Repository Structure and Releases

Open Glass Suite separates **private, in-progress development** from **publicly published project material**.

## Repository roles

### Private development repositories

Each component may have its own private repository for experiments, issues, implementation branches, tests, and CI. The initial browser experiment will be developed this way.

Repository names and build tools can vary by component. The private repositories are not intended to be mirrored automatically in full.

### Public suite repository

This repository, `LaszloK16/Open_Glass_Suite`, is the public entry point for the suite. As components become publishable, it is intended to contain:

- A directory for each published component, with its selected source files.
- Component-level documentation and changelogs.
- Release notes and downloadable artifacts in GitHub Releases.
- Cross-project documentation and consistent design guidance.

The public source tree may look like this **later**:

```text
Open_Glass_Suite/
├── README.md
├── docs/
├── browser/
│   ├── README.md
│   └── ...published source...
└── ...future published components...
```

This is a proposed structure, not a claim that the component directories or applications already exist.

## Intended release workflow

1. Develop and test a component in its private repository.
2. Choose a specific tested revision for publication.
3. Review a restricted set of source files and assets for publication; exclude secrets, private settings, and experimental content.
4. Copy the approved public source into the component's directory here.
5. Publish the corresponding build artifacts and release notes under a component-specific tag.
6. Continue independent development in the private repository.

Automation through GitHub Actions may be introduced after the first manual release path is proven. Publishing should require an explicit, reviewable decision rather than exposing everything pushed to a private development branch.

## Versioning

Each component is versioned independently. Planned tag format:

```text
browser-v0.1.0
other-component-v0.1.0
```

A public release should identify the exact component revision it corresponds to, list supported environments, include installation and removal instructions, and disclose important limitations.

## Licensing

A public-source license has not yet been selected. Before source publication, licensing and third-party dependency notices must be reviewed and included as appropriate.

## Current state

No automated publishing workflow, component source snapshot, or public build has been configured yet.
