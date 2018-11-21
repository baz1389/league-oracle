# The League Oracle
 
## Setup
* [Yarn](https://yarnpkg.com/en/docs/install)

1. Run `yarn install`.
2. Run `yarn start` and visit [locahost:3000](http://localhost:3000) to see
your appplication.

This application uses Yarn. **Do not use `npm install` commands**. Instead use the
equivalent [Yarn commands](https://yarnpkg.com/en/docs/usage).
 
 
### **[League of Legends Static Data API](https://developer.riotgames.com/static-data.html)**

#### Champions API Call
    
    http://ddragon.leagueoflegends.com/cdn/6.24.1/data/en_US/champion.json
    
#### Champions Response

```
{
	"type": "champion",
	"format": "standAloneComplex",
	"version": "6.24.1",
	"data": {
		"Aatrox": {
			"version": "6.24.1",
			"id": "Aatrox",
			"key": "266",
			"name": "Aatrox",
			"title": "the Darkin Blade",
			"blurb": "Aatrox is a legendary warrior, one of only five that remain of an ancient race known as the Darkin. He wields his massive blade with grace and poise, slicing through legions in a style that is hypnotic to behold. With each foe felled, Aatrox's ...",
			"info": {
				"attack": 8,
				"defense": 4,
				"magic": 3,
				"difficulty": 4
			},
			"image": {
				"full": "Aatrox.png",
				"sprite": "champion0.png",
				"group": "champion",
				"x": 0,
				"y": 0,
				"w": 48,
				"h": 48
			},
			"tags": ["Fighter", "Tank"],
			"partype": "BloodWell",
			"stats": {
				"hp": 537.8,
				"hpperlevel": 85.0,
				"mp": 105.6,
				"mpperlevel": 45.0,
				"movespeed": 345.0,
				"armor": 24.384,
				"armorperlevel": 3.8,
				"spellblock": 32.1,
				"spellblockperlevel": 1.25,
				"attackrange": 150.0,
				"hpregen": 6.59,
				"hpregenperlevel": 0.5,
				"mpregen": 0.0,
				"mpregenperlevel": 0.0,
				"crit": 0.0,
				"critperlevel": 0.0,
				"attackdamage": 60.376,
				"attackdamageperlevel": 3.2,
				"attackspeedoffset": -0.04,
				"attackspeedperlevel": 3.0
			}
		},
		...
    }
```

#### Version API Call

Note, most of the API calls include a version (e.g.`6.24.1`). If you don't want to hardcode this, you must also use the versions API call and pass it into the other API call URLs:

    https://ddragon.leagueoflegends.com/api/versions.json    

#### Version Response

```
["8.23.1","8.22.1","8.21.1","8.20.1","8.19.1","8.18.2","8.18.1",...]
```
