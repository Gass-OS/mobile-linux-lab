<div align="center">

# 🌌 Mobile Linux Lab

**A practical, evidence-first lab notebook for Linux desktop experiments on Android.**

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=111111)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=111111)
![Docs](https://img.shields.io/badge/Project-Documentation-777777?style=flat-square)

</div>

This repository organizes reproducible notes for exploring desktop Linux components on Android and Termux. It is documentation-first: results should be marked as tested, untested, or device-specific rather than assumed to work everywhere.

## Lab principles

1. **Record the environment.** Android version, device architecture, Termux source, package versions, display server, and graphics path matter.
2. **Separate facts from hypotheses.** Do not label a workflow as tested unless you ran it.
3. **Prefer reversible experiments.** Keep logs and explain how to undo configuration changes.
4. **Protect privacy.** Redact device identifiers, usernames, paths, and tokens from logs before publishing.
5. **Respect upstream licenses.** GNOME, Mutter, Mesa, and related projects retain their own licenses.

## Notebook

- [`docs/architecture.md`](docs/architecture.md) — high-level stack and vocabulary
- [`docs/test-log-template.md`](docs/test-log-template.md) — copyable experiment log
- [`docs/roadmap.md`](docs/roadmap.md) — staged roadmap and acceptance criteria

## Related GASS-OS projects

- [GNOME-Termux](https://github.com/Gass-OS/GNOME-Termux)
- [Termux-ludashi](https://github.com/Gass-OS/Termux-ludashi)
- [GASS-OS Termux Diagnostics](https://github.com/Gass-OS/gass-os-termux-diagnostics)
- [Termux Safe Bootstrap](https://github.com/Gass-OS/termux-safe-bootstrap)

## Contributing notes

A useful report includes the exact command, exit status, relevant versions, expected result, actual result, and a redacted log excerpt. Avoid publishing claims based on a single device as universal compatibility.

## License

MIT for the original documentation in this repository. Third-party names and trademarks belong to their respective owners.
