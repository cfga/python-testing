# Property-based and performance testing in Python

This repo showcases property-based and performance testing in Python done with:
- [pytest](https://docs.pytest.org/en/latest/)
- [pytest-benchmark](https://pytest-benchmark.readthedocs.io/en/latest/)
- [Hypothesis](https://hypothesis.readthedocs.io/en/latest/)

## Requirements

- Python >=3.7 (+ pip3 available on PATH)
- make

## Setting up the environment

This project uses [virtualenv](https://docs.python.org/3.7/tutorial/venv.html) to isolate the environment in which 
it is being run.

For instance, on MacOS, you would have to run:

```bash
$ python3 -m venv test-venv
$ source test-venv/bin/activate
```

Mind the possible necessity of using a different activation script, see `ls test-venv/bin`.

## Installing

This project uses setuptools. To install the project in-place along with its dependencies run:

`make install`

## Run tests
The tests are written using property-based testing library [Hypothesis](https://hypothesis.readthedocs.io/en/latest/). To run the tests:

`make test`

## Run benchmarks

Benchmarking is done with [pytest-benchmark](https://pytest-benchmark.readthedocs.io/en/latest/) library. To run the benchmarks:

`make bench`
