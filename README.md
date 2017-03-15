# StatStable

A Python wrapper for the StatStable API to easily retreive sports statistics.

## Installation

    pip install statstable

## Quick Start

```python
import statstable as ss

params = {
  'playerId': 'lebron-james',
  'fields':   ['date', 'MP', 'PTS']
}
stats = ss.getNBAStats(params)
```

`stats` will contain the following statistics:

```javascript
{
  "results": [
    {
        "date": "2017-03-01",
        "MP":   40.0,
        "PTS":  28
    },
    {
        "date": "2017-02-27",
        "MP":   37.2,
        "PTS":  24
    },
    {
        "date": "2017-02-23",
        "MP":   37.1,
        "PTS":  18
    },
    {
        // More stats
    }
  ],

  "request": {
    "playerId": "lebron-james",
    "fields": [
        "date", 
        "MP", 
        "PTS"
    ]
  },

  "url": "statstable.com/0ABCDE"
}
```

## Documentation

View StatStable's full documentation at https://statstable.com/docs
