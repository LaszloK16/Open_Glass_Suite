# Vision and Design Principles

Open Glass Suite (OGS) aims to give independently developed applications and existing software a coherent visual language without sacrificing the features that make those applications useful.

## Extend before replacing

The preferred order of implementation is:

1. Theme, extension, add-on, or plugin.
2. Extension plus a small native helper, only where operating-system access is needed.
3. Modification of an existing open-source application, when extension support is insufficient.
4. A standalone application, when the other options are impractical.

Compatibility, security updates, account features, and synchronization should be preserved wherever feasible.

## Visual direction

OGS aims for a restrained, dark, glass-like look:

- Transparent or translucent surfaces with clear visual hierarchy.
- Actual transparency to the desktop, where the host platform and rendering stack permit it.
- Optional blur, adjusted to remain legible and usable.
- Square or subtly rounded geometry, understated separators, and consistent spacing.
- Fully readable text, controls, media, and interactive elements.
- Per-application and, when useful, per-site controls and exclusions.

A shared specification can define colors and behavior, but each host platform should use an appropriate native implementation. There is no requirement to force all software into one UI framework.

## Engineering preferences

- Keep extensions and helpers small and narrowly scoped.
- Avoid unnecessary services, duplicate browser engines, and heavy wrapper runtimes.
- Make changes easy to enable, disable, and revert.
- Preserve the security boundaries of host applications.
- Respect performance: blur and transparency effects must be tested on real hardware.
- Prefer upstream compatibility and simple upgrades over permanent forks.
- Treat accessibility and reliable input behavior as requirements, not afterthoughts.

## Limits of the concept

A website's dark mode does not guarantee that its layout can be restyled safely. Complex pages may need site-specific rules or exclusions.

Browser transparency is also distinct from website CSS transparency. A Chrome extension alone cannot guarantee that the Windows desktop will show through the Chrome window. Any native composition technique must be tested before it becomes a supported feature.

These limitations should be documented honestly as experiments progress.
