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
| 4 | Message padding and blocks | In progress | [#4](https://github.com/kkostia/comp-theory-labs/issues/4) |
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
- [MD4 (RFC 1320)](https://www.rfc-editor.org/rfc/rfc1320): an older hash, used to compare byte order and the `F` and `G` functions.
- [UTF-8 (RFC 3629)](https://www.rfc-editor.org/rfc/rfc3629): how many bytes a character takes.
- [MD5 (RFC 1321)](https://www.rfc-editor.org/rfc/rfc1321): another hash whose constants come from a known formula.
- [Gilbert and Handschuh, Security Analysis of SHA-256 and Sisters](https://doi.org/10.1007/978-3-540-24654-1_13): an analysis of SHA-256 and weak simplified versions.
- [Nothing-up-my-sleeve number](https://en.wikipedia.org/wiki/Nothing-up-my-sleeve_number): why constants like these are used.
- [Bernstein et al., How to manipulate curve standards](https://ia.cr/2014/571): the limits of that idea.
- [Python floating point tutorial](https://docs.python.org/3/tutorial/floatingpoint.html): the 53 bits of precision in a float.
- [Sieve of Eratosthenes](https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes): a faster way to find primes.

## Author

Kostiantyn Panasenko — g00436001

AI assistance tools (ChatGPT and Claude) were used during this project.
