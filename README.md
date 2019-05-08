# ![LOGO](logo.png) WeGA **flow**ground Connector

## Description

A generated **flow**ground connector for the WeGA API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/weber-gesamtausgabe.de/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:44:52+03:00

## API Description

The OpenAPI documentation for the RESTful interface of the Carl-Maria-von-Weber-Gesamtausgabe. <br/> (No registration, authentication, or API key is required) <br/> For feedback or requests about this API please contact stadler@weber-gesamtausgabe.de or start the discussion at https://github.com/Edirom/WeGA-WebApp

## Authorization

This API does not require authorization.

## Actions

### Finds code samples by XML element

*Tags:* `Code Samples`

#### Input Parameters
* `element` - _required_ - The XML element to search for
* `namespace` - _optional_ - The element namespace. Defaults to the TEI namespace
* `docType` - _optional_ - The WeGA document type
* `offset` - _optional_ - Position of first item to retrieve (starting from 1)
* `limit` - _optional_ - Number of items to retrieve (200 max)

### Lists all documents

> The Documents endpoint returns a list of all documents from the WeGA digital edition.

*Tags:* `Documents`

#### Input Parameters
* `docType` - _optional_ - The WeGA document type
* `offset` - _optional_ - Position of first item to retrieve (starting from 1)
* `limit` - _optional_ - Number of items to retrieve (200 max)

### Finds documents by author

> This endpoint returns a list of documents by a given author - optionally filtered by document type

*Tags:* `Documents`

#### Input Parameters
* `authorID` - _required_ - The author ID to search for. Accepted ID formats are WeGA, e.g. A002068 or http://weber-gesamtausgabe.de/A002068, VIAF, e.g. http://viaf.org/viaf/310642461, or  GND, e.g. http://d-nb.info/gnd/118629662

* `docType` - _optional_ - The WeGA document type
* `offset` - _optional_ - Position of first item to retrieve (starting from 1)
* `limit` - _optional_ - Number of items to retrieve (200 max)

### Finds documents by date

> This endpoint returns a list of documents related to the given date - optionally filtered by document type.

*Tags:* `Documents`

#### Input Parameters
* `fromDate` - _required_ - The min date to search for
* `toDate` - _optional_ - The max date to search for
* `docType` - _optional_ - The WeGA document type
* `offset` - _optional_ - Position of first item to retrieve (starting from 1)
* `limit` - _optional_ - Number of items to retrieve (200 max)

### Finds documents by reference

> This endpoint returns a list of documents that reference a particular docID - optionally filtered by document type.

*Tags:* `Documents`

#### Input Parameters
* `docID` - _required_ - The document ID that is to be mentioned. Accepted ID formats are WeGA, e.g. A002068 or http://weber-gesamtausgabe.de/A002068, VIAF, e.g. http://viaf.org/viaf/310642461, or  GND, e.g. http://d-nb.info/gnd/118629662

* `docType` - _optional_ - The WeGA document type
* `offset` - _optional_ - Position of first item to retrieve (starting from 1)
* `limit` - _optional_ - Number of items to retrieve (200 max)

### Returns documents by ID

> This endpoint returns documents, indicated by an ID.<br/>
>  Accepted ID formats are WeGA, e.g. A002068 or http://weber-gesamtausgabe.de/A002068, VIAF, e.g. http://viaf.org/viaf/310642461, or  GND, e.g. http://d-nb.info/gnd/118629662

*Tags:* `Documents`

#### Input Parameters
* `docID` - _required_ - The document identifier to search for

## License

**flow**ground :- Telekom iPaaS / weber-gesamtausgabe-de-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
