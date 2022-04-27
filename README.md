# Emofid Investment Simulator API Documantation

## Request:

```
value (Toman): min: 1000000 - max: 1000000000
period (Years): 1 | 3 | 5 | 7
risk: low | medium | high
```

Example:

```
/?value=20000000&period=3&risk=medium
```


## Response

```json
{
    "return": {
        "value": 152000000,
        "percent": 1819,
    },
    "distribution": [
        {
            "name": "صندوق های سهامی",
            "percent": 40
        },
        {
            "name": "صندوق های درآمد ثابت",
            "percent": 30
        },
        {
            "name": "صندوق طلا",
            "percent": 30
        },
    ],
    "data": [
        {
            "id": "invested",
            "name": "پرتفوی پیشنهادی",
            "prices": [
                {
                    "date": "2016-01-15",
                    "value": 456300
                },
                {
                    "date": "2016-01-16",
                    "value": 456590
                },
            ]
        },
        {
            "id": "house",
            "name": "قیمت مسکن",
            "prices": [
                {
                    "date": "2016-01-15",
                    "value": 456300
                },
                {
                    "date": "2016-01-16",
                    "value": 456590
                },
            ]
        },
    ]
}
```