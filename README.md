# Airbus Defence and Space Geo Processing APIs


## Geo Process API

### Endpoints notices

#### `/api/v1/describe`

##### input
This field defines geoprocess' input payload, that is to say the json content that someone want to post to `/api/v1/jobs` must be compliant with `describe.input` schema. This JSON schema may rely on standard json-schemas definitions :
* [image](2.0/definitions/image.json)

Example :
* [`describe.input` schema](2.0/examples/geoprocess.describe.input.schema.json)
* [POST payload](2.0/examples/geoprocess.input.json))

##### inputCapabilities
This field defines geoprocess' supported input values. It is formatted as a JSON that must be compliant with [standard json-schema](2.0/definitions/inputCapabilities.json) (or an extension of this schema).

As a result, a geoprocess engine compliant with [standard json-schema](2.0/definitions/inputCapabilities.json) (or an extension of this schema) is able to parse these capabilities and check if it can support this geoprocess or not.

Example :
* [example](2.0/examples/geoprocess.inputCapabilities.json)

##### output
This field defines geoprocess' ouput payload, that is to say the json response that someone will receive after posting to `/api/v1/jobs` will be compliant with `describe.output` schema. This JSON schema may rely on standard json-schemas definitions :
* [image](2.0/definitions/image.json)
* [geojson](https://geojson.org/schema/FeatureCollection.json)

Example :
* [`describe.output` schema](2.0/examples/geoprocess.describe.output.schema.json)
* [POST response](2.0/examples/geoprocess.output.json))

##### outputCapabilities
This field defines geoprocess' possible output values. It is formatted as a JSON that will be compliant with [standard json-schema](2.0/definitions/outputCapabilities.json) (or an extension of this schema).

As a result, a geoprocess engine compliant with [standard json-schema](2.0/definitions/outputCapabilities.json) (or an extension of this schema) is able to parse these capabilities and check if it can support this geoprocess or not.

Example :
* [example](2.0/examples/geoprocess.outputCapabilities.json)


## Geo Processes Management API


## Versions

1.0.1

## Changelog

1.0.1 : Bug fix release
 * Remove sibling values
 * Remove unrelevant dataset search criterion for jobs
 * Factorize model schemas using open api inheritance
 * Fix page id and size type

1.0 : First version
