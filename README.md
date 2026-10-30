# Computational Theory: SHA-256

This is my project for the Computational Theory module at ATU Galway.
I am building the [SHA-256](https://doi.org/10.6028/NIST.FIPS.180-4) hash function step by step using Python and NumPy, with short explanations and tests in a Jupyter notebook.

The work is still in progress.

## Contents

- [Repository structure](#repository-structure)
- [Progress](#progress)
- [How to run](#how-to-run)
- [Dependencies](#dependencies)
- [References](#references)
- [Use of AI](#use-of-ai)
- [Author](#author)

## Repository structure

| File | Purpose |
| --- | --- |
| `problems.ipynb` | The notebook with all my work |
| `requirements.txt` | Python packages needed to run the notebook |
| `AGENTS.md` | Rules for AI tools used in this repository |
| `.gitignore` | Files that Git should not track |

## Progress

| Problem | Topic | Status | Issue |
| --- | --- | --- | --- |
| 1 | Data representations | Complete | [#1](https://github.com/kkostia/comp-theory-labs/issues/1) |
| 2 | Bitwise functions | Complete | [#2](https://github.com/kkostia/comp-theory-labs/issues/2) |
| 3 | Round constants | Complete | [#3](https://github.com/kkostia/comp-theory-labs/issues/3) |
| 4 | Message padding and blocks | Not started | [#4](https://github.com/kkostia/comp-theory-labs/issues/4) |
| 5 | Compression function | Not started | [#5](https://github.com/kkostia/comp-theory-labs/issues/5) |
| 6 | Full SHA-256 | Not started | [#6](https://github.com/kkostia/comp-theory-labs/issues/6) |

## How to run

Install [Python](https://www.python.org/) and [Git](https://git-scm.com/), then run:

```sh
git clone https://github.com/kkostia/comp-theory-labs.git
cd comp-theory-labs
python -m pip install -r requirements.txt
jupyter notebook problems.ipynb
```

In Jupyter, run the cells from top to bottom, because later problems use functions from earlier ones.

## Dependencies

| Package | Purpose |
| --- | --- |
| [NumPy](https://numpy.org/) | 32-bit unsigned integers and arrays |
| [Jupyter Notebook](https://jupyter.org/) | Opening and running the notebook |
| [ipykernel](https://ipykernel.readthedocs.io/) | Running Python inside Jupyter |

## References

- [Secure Hash Standard (FIPS 180-4)](https://doi.org/10.6028/NIST.FIPS.180-4): the official definition of SHA-256.
- [NumPy scalar types](https://numpy.org/doc/stable/reference/arrays.scalars.html): how `uint32` works.
- [Python `int` methods](https://docs.python.org/3/library/stdtypes.html#int.from_bytes): converting between integers and big-endian bytes.
- [Course notes on prime numbers](https://github.com/ianmcloughlin/computational-theory/blob/main/notes/prime-numbers.ipynb): the approach I followed for `primes(n)`.

## Use of AI

I used [ChatGPT](https://chatgpt.com/) to help with Problem 1.
I used [Claude](https://claude.ai/) to review Problems 1 to 3, add code comments, add the plain Python check for the sigma functions, change how the constants are printed, write the notebook introduction, and tidy this README.

## Author

Kostiantyn Panasenko — g00436001
