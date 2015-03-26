# PyJNE


## Quickstart
```python
from jne import Jne

jne = Jne(api_key='8ab4dfdcf40d6c09f22704342907d804', username='TESTAPI')

# Get from code
jne.get_from_code('jakarta')

# Get target code
jne.get_target_code('jakarta')

# Check tariff
jne.check_tariff(city_from='CGK10000', city_to='CBN10000', weight=1)

# Tracking
jne.tracking(airbill='123455683982777')

```

For pretty print response, add `pretty_print=True`
```python
jne.get_from_code('jakarta', pretty_print=True)
```


## Test
```
python -m unittest discover
```
