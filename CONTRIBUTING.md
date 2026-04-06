# Contributing to PLFM_RADAR (AERIS-10)

Thanks for your interest in the project! This guide covers the basics
for getting a change reviewed and merged.

## Getting started

1. Fork the repository and create a topic branch from `develop`.
2. Keep generated outputs (Vivado projects, bitstreams, build logs)
   out of version control — the `.gitignore` already covers most of
   these.

## Repository layout

| Path | Contents |
|------|----------|
| `4_Schematics and Boards Layout/` | KiCad schematics, Gerbers, BOM/CPL |
| `9_Firmware/9_2_FPGA/` | Verilog RTL, constraints, testbenches, build scripts |
| `9_Firmware/9_2_FPGA/formal/` | SymbiYosys formal-verification wrappers |
| `9_Firmware/9_2_FPGA/scripts/` | Vivado TCL build & debug scripts |
| `9_Firmware/9_3_GUI/` | Python radar dashboard (Tkinter + matplotlib) |
| `docs/` | GitHub Pages documentation site |

## Before submitting a pull request

- **Python** — verify syntax: `python3 -m py_compile <file>`
- **Verilog** — if you have Vivado, run the relevant `build*.tcl`;
  if not, note which scripts your change affects
- **Whitespace** — `git diff --check` should be clean
- Keep PRs focused: one logical change per PR is easier to review

## Areas where help is especially welcome

See the list in [README.md](README.md#-contributing).

## Questions?

Open a GitHub issue — that way the discussion is visible to everyone.
