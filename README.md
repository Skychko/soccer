# Soccer teams and leagues

## Description

The field `"search"` (leagues, teams) is utilized to combine current data with data from a third-party source. For instance, if you have a schedule of matches in the format [TEAM NAME 1] - [TEAM NAME 2], and you wish to display this data along with team logos.

Team and league logos are raw. It's supposed they will be precompiled for production usage (I.e. be automatically resized and combined to sprites).

## Structure:

* `./leagues`
    * `./logos/[id].png` - league logo
    * `./index.json` - leagues list
```json
[
    {
        "id": "[internal league ID]",
        "name": "[league name]",
        "country": "[league country, if it exists]",
        "search": "[league name variations; lowercase]"
    }
]
```
* `./teams`
    * `/logos/[id].png` - team logo
    * `/index.json` - teams list
```json
[
    {
        "id": "[internal team ID]",
        "name": "[team name]",
        "country": "[team country]",
        "search": "[team name variations; lowercase]"
    }
]
```
