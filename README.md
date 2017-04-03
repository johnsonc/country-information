![The Basetrip](http://i.imgur.com/91EWQao.png)

# Country data
> Get information for 230+ countries in structured format.

## 🚀 Getting started
This repository contains information about 232 countries in `JSON` format, including country names, flags, maps, capital cities and more.

### Example
```json
{
  "slug": "france",
  "name": {
    "common": "France",
    "official": "French Republic"
  },
  "code": {
    "alpha2": "FR",
    "alpha3": "FRA",
    "numeric": "250"
  },
  "languages": [
    {
      "name": "French",
      "type": "OFFICIAL",
      "code": {
        "alpha2": "fr",
        "alpha3": "fra"
      }
    }
  ],
  "location": {
    "region": "EUROPE",
    "subregion": "WESTERN_EUROPE",
    "geoJson": "https://raw.githubusercontent.com/the-basetrip/country-information/master/dist/maps/FR.geo.json"
  },
  "capital": {
    "name": "Paris",
    "coordinates": {
      "latitude": 48.856614,
      "longitude": 2.3522219
    },
    "timeZone": "Europe/Paris"
  },
  "unions": [
    "EUROPEAN_UNION",
    "EUROPEAN_ECONOMIC_AREA",
    "SCHENGEN_AREA"
  ],
  "flag": {
    "png": "https://raw.githubusercontent.com/the-basetrip/country-information/master/dist/flags/FR.png",
    "svg": "https://raw.githubusercontent.com/the-basetrip/country-information/master/dist/flags/FR.svg",
    "emoji": "🇫🇷"
  },
  "isSovereignState": true,
  "measurementSystem": "METRIC_SYSTEM",
  "wikipediaUrl": "https://en.wikipedia.org/wiki/France"
}
```

### Structure
| Name | Type | Description
| --- | --- | --- |
| slug | String | Sanitized country name (using only `a-z` and `-` as a word separator)
| name.common | String | Common country name - usually the one displayed on the UI
| name.official	| String | Official country name
| code.alpha2 | String | [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) two-letter country code
| code.alpha3 | String | [ISO 3166-1 alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) three-letter country code
| code.numeric | String | [ISO 3166-1 numeric](https://en.wikipedia.org/wiki/ISO_3166-1_numeric) three-digit country code
| languages.name | String | Language name
| languages.type | String | Language type (for now only `OFFICIAL`)
| languages.code.alpha2 | String | Language [ISO 639-1](https://en.wikipedia.org/wiki/ISO_639-1) two-letter code
| languages.code.alpha3 | String | Language [ISO 639-3](https://en.wikipedia.org/wiki/ISO_639-3) three-letter code
| location.region | String | Country region (`AFRICA`, `AMERICAS`, `ASIA`, `EUROPE` or `OTHER`)
| location.subregion | String | Country subregion (`AUSTRALIA_AND_NEW_ZEALAND`, `CARIBBEAN`, `CENTRAL_AMERICA`, `CENTRAL_ASIA`, `EASTERN_AFRICA`, `EASTERN_ASIA`, `EASTERN_EUROPE`, `MELANESIA`, `MICRONESIA`, `MIDDLE_AFRICA`, `NORTHERN_AFRICA`, `NORTHERN_AMERICA`, `NORTHERN_EUROPE`, `POLYNESIA`, `SOUTH_AMERICA`, `SOUTH_EASTERN_ASIA`, `SOUTHERN_AFRICA`, `SOUTHERN_ASIA`, `SOUTHERN_EUROPE`, `WESTERN_AFRICA`, `WESTERN_ASIA`, `WESTERN_EUROPE`)
| location.geoJson | String | URL of GeoJSON data
| capital.name | String | Name of the capital city
| capital.coordinates.latitude | double | Latitude in decimal degrees
| capital.coordinates.longitude | double | Longitude in decimal degrees
| capital.timeZone | String | Time zone ID ([full list](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones))
| unions | String[] | Unions which country is part of (includes `EUROPEAN_UNION`, `EUROPEAN_ECONOMIC_AREA`, `SCHENGEN_AREA`)
| flag.png | String | URL of country flag in `PNG` format (`512px` in width)
| flag.svg | String | URL of country flag in `SVG` format
| flag.emoji | String | Emoji (UTF-8 character) representing the country flag
| isSovereignState | boolean | Determines whether country is sovereign state or not (i.e. constituent state, unincorporated and organized territory etc.)
| measurementSystem | String | `METRIC_SYSTEM`, `UNITED_STATES_CUSTOMARY_SYSTEM`, `IMPERIAL_SYSTEM`, `BURMESE_SYSTEM`
| wikipediaUrl | String | URL of Wikipedia entry about the country

## Contributing
The best way to contribute is to create issues or pull requests right here on Github. You can also reach us through [our website](https://www.thebasetrip.com/en/api) via chat widget.

## Support
Please open an issue and describe your situation in detail. We will respond as soon as we can.
For an API, commercial support and more extensive database please contact us at [The Basetrip API](https://www.thebasetrip.com/en/api) page.

## Who built this?
The repository is maintaned by [The Basetrip](https://www.thebasetrip.com). We have built the B2C showcase website as well as commercial B2B API to provide easy & accurate country travel information.

## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a><br />This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

**Sources**: [Wikipedia](https://www.wikipedia.org), [CLDR](http://cldr.unicode.org), [World Borders Dataset](http://thematicmapping.org/downloads/world_borders.php)
