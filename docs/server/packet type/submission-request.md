# Submission

## Judge server expectation

```python
Submission = NamedTuple(
    'Submission',
    [
        ('id', int),
        ('problem_id', str),
        ('language', str),
        ('source', str),
        ('time_limit', float),
        ('memory_limit', int),
        ('short_circuit', bool),
        ('meta', Dict),
    ],
)

req = {
    "name": "submission-request",
    "submission-id": "1", # Server self-manage id
    
    "problem-id": "aplusb", # Must match id in problem root defined in judge env
    "language": "cpp", # All availible in ./dmoj/executors
    "source": "SOURCE_CODE", # The fucking source code
    "time-limit": 1.0, # float, in seconds
    "memory-limit": 256, # int, in KB
    "short-circuit": "?", # Lmao what is this
    "meta": "?",
}
```
