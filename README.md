# warframe-worldstate-data
A repository of Warframe data for use with warframe-worldstate-parser

## Installation
```
npm install --save warframe-worldstate-data@latest
```

## Usage

```javascript
var worldstateData = require('warframe-worldstate-data');
var nodes = worldstateData.solNodes;

var erpo = nodes['SolNode903'];
var erpoEnemyType = erpo.enemy;
var erpoName = erpo.value;
var erpoMission = erpo.type;
```

## Available data and formatting

JSON | Data Accessor | Description
--- |--- | --- 
`conclaveData.json` | `conclave` | Stores conclave data for modes and categories
`eventsData.json` | `events` | Stores event strings. May be deprecated when languages.json is more complete.
`factionsData.json`|`factions`|Stores faction strings for identifying each faction
`fissureModifiers.json`|`fissureModifiers`|Fissure tier assignments corresponding to era names
`languages.json`|`languages`|General string storage for converting worldstate strings to display strings
`missionTypes.json`|`missionTypes`|Types of missions, ex.: `MT_EXCAVATE` corresponds to `Excavation`
`operationTypes.json`|`operationTypes`|Operation string conversions for global modifiers
`persistentEnemyData.json`|`persistentEnemy`|Persistent enemy data mappings. Currently only acolytes.
`relics.json`|`relics`|Relic information pertaining to what relics prime parts are derived from.
`solNodes.json`|`solNodes`|Data for each node in the solar system. Currently includes node name, base enemy type, and base mission type
`syndicateData.json`|`syndicates`|Mappings for worldstate syndicate names to displayable syndicate names.
`upgradeTypes.json`|`upgradeTypes`|Upgrade types for global modifiers.
