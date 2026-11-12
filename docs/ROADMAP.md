# Roadmap

This roadmap records intended directions, **not release commitments or target dates**. Priorities may change as prototypes expose technical limitations.

## Phase 1 — Foundation

- [x] Establish the Open Glass Suite name and extension-first approach.
- [x] Create the public suite repository and initial documentation.
- [ ] Select a suitable license before publishing reusable code.
- [ ] Define the initial shared theme tokens and defaults.
- [ ] Establish the first component's private development repository.

## Phase 2 — Chrome transparency feasibility

- [ ] Build a small Chrome extension that identifies and restyles webpage backgrounds.
- [ ] Test CSS background removal and basic site compatibility.
- [ ] Prototype a minimal Windows-native transparency helper **if required**.
- [ ] Test whether the Chrome compositor can expose actual desktop windows through webpage regions.
- [ ] Measure interaction, scrolling, video, GPU, and window-resizing behavior.
- [ ] Decide whether the extension/helper approach is sufficiently robust to continue.

**Important:** Genuine desktop transparency through an unmodified Chrome window remains an unproven goal. A successful CSS-only mockup is not proof of desktop transparency.

## Phase 3 — First usable component (conditional)

Only if the feasibility tests justify it:

- [ ] Add user-controlled opacity and styling presets.
- [ ] Keep text, images, and media readable.
- [ ] Add per-site overrides and an easy disable/restore mechanism.
- [ ] Test browser restarts, updates, multiple windows, and multiple monitors.
- [ ] Publish source, usage instructions, known limitations, and the first tagged release.

## Future directions

Other applications may receive Open Glass themes, add-ons, plugins, or native helpers. No specific additional application is committed yet. Projects should be added when there is a concrete use case and an implementation path that does not introduce unnecessary maintenance.

See [Vision](VISION.md) for design and engineering priorities.
