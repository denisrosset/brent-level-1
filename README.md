# Brent algorithm

## To install

Brent's algorithm requires `Python 3.8` and the [rich](https://github.com/Textualize/rich) library.

```bash
pip install -r requirements.txt
```

Then run the following in a Python shell:

```python
import brent
import math
settings = brent.Settings(x_rel_tol=1e-12, x_abs_tol=1e-12, y_tol=1e-12, verbose=True)
f = math.cos
brent.brent(f, 0.0, 3.0, settings)
```

or open the example notebook `example.ipynb`.


## To develop

We use [VS Code](https://code.visualstudio.com/), the Black/isort/pylint tools. To install them, run:

```bash
pip install -r requirements_dev.txt
```
