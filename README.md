# SVO API
API to download [Spanish Virtual Observatory](http://svo2.cab.inta-csic.es/theory/fps/index.php?mode=browse) filters.

[![repo](https://img.shields.io/badge/GitHub-temuller%2Fsvo_api-blue.svg?style=flat)](https://github.com/temuller/svo_api)
[![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/svo_api/blob/master/LICENSE)
![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
[![PyPI](https://img.shields.io/pypi/v/svo_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/svo_api/)
[![DOI](https://zenodo.org/badge/643973679.svg)](https://zenodo.org/badge/latestdoi/643973679)


## Installation

It is recommended to install ``svo_api`` from pip:

```python
pip install svo_api
```
or it can be installed from source in the usual way.

## Usage Example

You can obtain the list of available facilities in SVO in one command:

```python
get_facilities()
```

Many facilities can have multiple filters sets, e.g. for different instruments and telescopes. These can be obtained as follows:

```python
facility = 'Paranal'
get_filters_sets(facility)
```

To download the filters, run the following command:

```python
facility = 'Paranal'
filter_sets = 'HAWKI'  # if not specified, download all the filters sets
download_filter(facility, filter_sets)
```

## Contributing
To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).

## Citing SVO API

If you make use of this code, please cite it:

```code
@software{tomas_e_muller_bravo_2023_7957749,
  author       = {Tomás E. Müller Bravo},
  title        = {temuller/svo\_api: First Release (for zenodo)!},
  month        = may,
  year         = 2023,
  publisher    = {Zenodo},
  version      = {v0.1.0-zenodo},
  doi          = {10.5281/zenodo.7957749},
  url          = {https://doi.org/10.5281/zenodo.7957749}
}
```
