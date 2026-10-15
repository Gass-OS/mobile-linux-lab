# Roadmap

This roadmap is a proposal, not a claim that the items are already implemented.

## Phase 1 — Baseline and reproducibility

- [ ] Record supported Android/Termux baseline
- [ ] Add redacted sample diagnostic report
- [ ] Standardize experiment logs
- [ ] Document the known-good software-rendering path

**Acceptance:** a new tester can collect a diagnostic report and reproduce the documented baseline without root.

## Phase 2 — Display and desktop integration

- [ ] Document Termux:X11 setup and recovery
- [ ] Track session startup/shutdown behavior
- [ ] Record D-Bus and audio integration requirements
- [ ] List known failures with logs and versions

**Acceptance:** setup instructions include prerequisites, verification commands, expected output, and recovery steps.

## Phase 3 — Graphics investigation

- [ ] Identify device/GPU-specific constraints
- [ ] Compare software rendering with available hardware paths
- [ ] Record frame-rate or responsiveness measurements with methodology
- [ ] Keep experimental driver overrides separate from the stable baseline

**Acceptance:** every performance claim includes device, versions, workload, rendering path, and measurement method.

## Phase 4 — Contributor quality

- [ ] Add issue templates
- [ ] Add shell syntax checks for scripts
- [ ] Add CI for documentation links where practical
- [ ] Review licensing and third-party attribution
