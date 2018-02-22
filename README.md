**C4Logger** saves useful informations about the use of C4.

## Permissions
- `c4logger.used` -- Get a message everytime someone uses a C4.
- `c4logger.connection` -- Get a message everytime someone connects / disconnects with C4 or Detonator Caps.

## Configuration
```json
{
  "Settings": {
    "Filters": {
      "Defuse": {
        "Enabled": true,
        "Max Time (Seconds)": 30
      },
      "Duplicate": {
        "Enabled": true,
        "Max Distance": 6,
        "Max Time (Seconds)": 3
      },
      "Self Harm": {
        "Enabled": true
      }
    },
    "Max Age (Days)": 7.0,
    "Players Near Radius": 100.0
  }
}
```

## Localization
```json
{
  "C4 - Used": "Player '{name}' used C4 at '{position}'.",
  "C4 - Disconnected": "Player '{name}' disconnected with:\nC4: {c4Count}\nDetonator Cap: {dCapCount}",
  "C4 - Connected": "Player '{name}' connected with {c4Count} x C4 and {dCapCount} x Detonator Cap."
}
```

## Example Data File
```json
[  
   {  
      "Date":"2016-04-11T22:33:00.8295262Z",
      "Position":"-2030.03 193.56 -1057.3",
      "Player":{  
         "Name":"Player One",
         "SteamId":"xxxxxxxxxxxxxxxxx",
         "C4":2,
         "Position":"-2027.85 195 -1057.81",
         "Distance":2.66,
         "Solidarity":{  
            "Clan":true,
            "Stake":true
         }
      },
      "Targets":[  
         {  
            "Online":true,
            "Name":"Player Two",
            "SteamId":"xxxxxxxxxxxxxxxxx",
            "C4":2,
            "Position":"-2027.85 195 -1057.81",
            "Distance":2.66,
            "Solidarity":{  
               "Clan":false,
               "Stake":false
            }
         }
      ],
      "Players Near":[  
         {  
            "Name":"Player Three",
            "SteamId":"xxxxxxxxxxxxxxxxx",
            "C4":0,
            "Position":"-2027.85 195 -1057.81",
            "Distance":1.25,
            "Solidarity":{  
               "Clan":true,
               "Stake":true
            }
         },
         {  
            "Name":"Player Four",
            "SteamId":"xxxxxxxxxxxxxxxxx",
            "C4":0,
            "Position":"-2027.85 195 -1057.81",
            "Distance":3.11,
            "Solidarity":{  
               "Clan":true,
               "Stake":false
            }
         },
        {  
            "Name":"Player Five",
            "SteamId":"xxxxxxxxxxxxxxxxx",
            "C4":1,
            "Position":"-2027.85 195 -1057.81",
            "Distance":6.66,
            "Solidarity":{  
               "Clan":false,
               "Stake":false
            }
         }
      ]
   }
]
```
