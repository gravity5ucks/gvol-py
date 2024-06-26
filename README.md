# GVol

[![Latest Version](https://img.shields.io/pypi/v/gvol.svg)](https://pypi.org/project/gvol/)
[![Supported Python Versions](https://img.shields.io/pypi/pyversions/gvol.svg)](https://pypi.org/project/gvol/)
[![Main Workflow](https://github.com/genesis-volatility/gvol-py/actions/workflows/main.yml/badge.svg)](https://github.com/genesis-volatility/gvol-py/actions/workflows/main.yml)
[![Documentation Status](https://readthedocs.org/projects/gvol/badge/?version=latest)](https://gvol.readthedocs.io/en/latest/?badge=latest)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

GVol is a Python library to access the [GVol API](https://docs.gvol.io/).

---

**Documentation**: [https://gvol.readthedocs.io/en/latest/index.html](https://gvol.readthedocs.io/en/latest/index.html)

---

## Install

```bash
pip install gvol
```

## Demo

```python
from gvol import GVol
from gvol import Amberdata

gvol_client = GVol(header='x-oracle', gvol_api_key="ENTER YOUR API KEY HERE")

options_orderbook = gvol_client.options_orderbook(
    symbol="BTC", exchange="deribit"
)

print(options_orderbook)

amberdata_client = Amberdata(api_key="ENTER YOUR AD API KEY HERE")
amberdata_client.get_term_structure(currency='BTC', exchange='deribit')


```
