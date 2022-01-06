# GVol

[![Main workflow](https://github.com/genesis-volatility-public/gvol/actions/workflows/main.yml/badge.svg)](https://github.com/genesis-volatility-public/gvol/actions/workflows/main.yml)
[![Documentation Status](https://readthedocs.org/projects/gvol/badge/?version=latest)](https://gvol.readthedocs.io/en/latest/?badge=latest)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

---

**Documentation**: [https://gvol.readthedocs.io/en/latest/index.html](https://gvol.readthedocs.io/en/latest/index.html)

---

## Install

```bash
pip install git+ssh://git@github.com/genesis-volatility-public/gvol@main
```

## Demo
```python
from gvol import GVol

gvol_client = GVol("gvol_api_key")

orderbook_skew_strike = gvol_client.CurrentOrderbookSkewStrike(
    symbol="BTC", exchange="deribit"
)

print(orderbook_skew_strike)
```