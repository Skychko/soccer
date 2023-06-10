# Soccer teams and leagues

## Structure:

* `./leagues`
    * `./logos/[id].png` - league logo
    * `./index.json` - leagues list
```json
[
    ...,
    {
        "id": "[internal league ID]",
        "name": "[league name]",
        "country": "[league country, if it exists]"
        "search": "[league name variations; lowercase; used to merge with 3rd party data by league name]",
    },
    ...
]
```
* `./teams`
    * `/logos/[id].png` - team logo
    * `/index.json` - teams list
```json
[
    ...,
    {
        "id": "[internal team ID]",
        "name": "[team name]",
        "country": "[team country]",
        "search": "[team name variations; lowercase; used to merge with 3rd party data by team name]"
    },
    ...
]
```
