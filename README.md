# Darglint

A limited docstring linter which checks that function/method parameters
are defined in their docstrings.

Darglint is in a very early stage, and fails for a lot of things.
Certain features, such as a robust command-line interface, still
do not exist.

## Installation

Clone the repository:

```
git clone https://github.com/terrencepreilly/darglint.git
```

`cd` into the directory, create a virtual environment (optional), then setup:

```
cd darglint/
virtualenv -p python3.6 .env
source .env/bin/activate
pip install -e .
```

## Usage

Given a python source file, `serializers.py`, you would check the docstrings
as follows:

```
darglint serializers.py
```

## Features planned and implemented

- [x] Function definitions can be checked.
- [ ] Methods definitions of top-level class can be checked.
- [ ] Line number printout for function/method definition.
- [ ] Syntastic support.
- [ ] Add support for type hints. (By replacing `redbaron`?)

## Development

Install `darglint` as above. To run tests,

```
python setup.py test
```

Or, install `pytest` manually, `cd` to the project's root directory,
and run

```
pytest
```

Contributions welcome.
