# Numerical Optimisation

University of Copenhagen · MSc Economics, elective from DIKU · Spring 2026 · 7.5 ECTS  
Course code NDAA09009U · [Course description](https://kurser.ku.dk/course/ndaa09009u)

Unconstrained and constrained optimisation, covering line search and trust-region methods, Newton and quasi-Newton methods such as BFGS, conjugate gradients and the KKT conditions. The five hand-ins combine proofs with Python implementations tested on benchmark functions.

## Contents

| Folder | Contents |
| --- | --- |
| `Handin1/ … Handin5/` | Hand-ins with the report as `main.tex` and `main.pdf`, plus notebooks and Python code |
| `weekly-notes/weekly-note-1/` | Weekly note 1, `main.tex` and `main.pdf` |
| `Old_handin/` | Earlier compiled hand-ins |

## Topics

- Newton and quasi-Newton methods
- Line search and the Wolfe conditions
- BFGS and superlinear convergence
- Conjugate gradients
- Equality-constrained optimisation and tangent cones

## Tools

Python, uv, LaTeX

## Build

Each LaTeX source sits next to its PDF. Rebuild a PDF from its folder with:

```bash
tectonic -Z continue-on-errors main.tex
```

## Setup

#### Install Homebrew (for Emil & Mathilde)

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### Install uv (for Emil & Mathilde)

```bash
brew install uv
```

uv is a fast Python package installer and resolver, written in Rust. It is used for reproducibility because it ensures consistent dependency versions across environments by locking dependencies in a uv.lock file.

#### Clone the Repository

```bash
git clone git@github.com:rohde01/numerical-optimisation.git
```

#### Sync Dependencies

```bash
uv sync
```