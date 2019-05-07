# ![LOGO](logo.png) LotaData **flow**ground Connector

## Description

A generated **flow**ground connector for the LotaData API (version 2.0.0).

Generated from: https://api.apis.guru/v2/specs/lotadata.com/2.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:42:47+03:00

## API Description

Access the most exhaustive, accurate and up-to-date collection of global and hyper-local geocoded events and activities across a wide range of categories and genres

## Authorization

Supported authorization schemes:
- API Key
## Actions

### Find event occurrences in the area. Returns results at specific place and time, event groups are expanded for every occurrence.

*Tags:* `Events`

#### Input Parameters
* `category` - _optional_ - List of required EventCategory ids (Tier 1)
* `activity` - _optional_ - List of required activity type ids (compliment to category)
* `ambience` - _optional_ - List of required ambience ids
* `genre` - _optional_ - List of required genre ids
* `name` - _optional_ - Matching on event and place names
* `q` - _optional_ - Text query matching titles, description, various text, tags, category
* `from_day` - _optional_ - Start on or after date specified (2015-10-16)
* `to_day` - _optional_ - Start on or before date specified (2015-10-16)
* `capacity_min` - _optional_ - Min capacity at location
* `capacity_max` - _optional_ - Min capacity at location
* `center` - _optional_ - latitude,longitude of the origin point
* `radius` - _optional_ - Distance from origin in meters
* `bbox` - _optional_ - Corner of a bounding box (lat,lng). Requires 0 or 2 pairs
* `polygon` - _optional_ - Closed custom polygon. Ordered list of lat,lng pairs
* `within` - _optional_ - Search within specified geopolitical place id
* `offset` - _optional_ - Return results starting at specified offset
* `limit` - _optional_ - Max results to return
* `fieldset` - _required_ - Return results starting at specified offset (summary, context, detail)
    Possible values: summary, detail, context, minicontext.

### Get Specific event details.

*Tags:* `Events`

#### Input Parameters
* `id` - _required_ - event @id
* `fieldset` - _optional_
    Possible values: summary, detail, context, minicontext.

### Venues, landmarks, regions, these are all places to search.

*Tags:* `Places`

#### Input Parameters
* `category` - _optional_ - List of required PlaceCategory ids (Tier 1)
* `function` - _optional_ - List of required PlaceFunction ids (Tier 2)
* `ambience` - _optional_ - List of required ambience ids
* `tag` - _optional_ - List of required tags
* `type` - _optional_ - Specific PlaceType to return
* `name` - _optional_ - Match on place names
* `exact` - _optional_ - Require an exact name match
* `capacity_min` - _optional_ - Min capacity at location
* `capacity_max` - _optional_ - Min capacity at location
* `street` - _optional_ - Address of the place or street component of the address
* `locality` - _optional_ - city, town, or neighborhood of the place
* `region` - _optional_ - region or state
* `postal_code` - _optional_ - Postal or zip code
* `country` - _optional_ - country component of the address
* `center` - _optional_ - latitude,longitude of the origin point
* `radius` - _optional_ - Distance from origin in meters
* `bbox` - _optional_ - Corner of a bounding box (lat,lng). Requires 0 or 2 pairs
* `polygon` - _optional_ - Closed custom polygon. Ordered list of lat,lng pairs
* `within` - _optional_ - Search within specified geopolitical place id
* `offset` - _optional_ - Return results starting at specified offset
* `limit` - _optional_ - Max results to return
* `fieldset` - _required_ - Return results starting at specified offset (summary, context, detail)
    Possible values: summary, detail, context.

### Get specific place details

*Tags:* `Places`

#### Input Parameters
* `id` - _required_ - place @id
* `fieldset` - _optional_
    Possible values: summary, detail, context, minicontext.

## License

**flow**ground :- Telekom iPaaS / lotadata-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
