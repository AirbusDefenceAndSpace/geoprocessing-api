# Airbus Defence and Space Geo Processing APIs

## Geo Process API

[REST](https://en.wikipedia.org/wiki/Representational_state_transfer) API to be implemented by processing components that plugs to the Airbus-DS processing tools.
Provided as [OpenAPI](https://en.wikipedia.org/wiki/OpenAPI_Specification) specification : [api_geo_process.yaml](api_geo_process.yaml).

### Geo Process API templates

Templates specifies Geo Process API for a kind of process.

Two classes of processing are definied :

* Object detection
* Change detection

Templates are provided as JSON schemas for the following endpoints:

* Geo Process API describe endpoint
* Geo Process API config endpoint
* Input of Geo Process API jobs endpoint
* if no output of Geo Process API jobs endpoint, GeoJSON with a FeatureCollection is expected

#### Object detection

* Describe endpoint schema : [tile-object-detection-describe.json](tile-object-detection-describe.json)
* Config endpoint schema : [tile-object-detection-config.json](tile-object-detection-config.json)
* Jobs endpoint input schema : [tile-object-detection-input.json](tile-object-detection-input.json)

#### Change detection

* Describe endpoint schema : [tile-change-detection-describe.json](tile-change-detection-describe.json)
* Config endpoint schema : [tile-change-detection-config.json](tile-change-detection-config.json)
* Jobs endpoint input schema : [tile-change-detection-input.json](tile-change-detection-input.json)

## Geo Processes Management API

[REST](https://en.wikipedia.org/wiki/Representational_state_transfer) API that allows external applications that are allowed to manage processes and job execution by Airbus-DS processing tools.
Provided as [OpenAPI](https://en.wikipedia.org/wiki/OpenAPI_Specification) specification : [api_geo_processes_manager.yaml](api_geo_processes_manager.yaml).

### Job input data

As the API is generic to process several kind of processes, templates specifies Geo Processes Manager API job input for a kind of process.

Two kinds of process are defined with there associated JSON schema for the jobs creation endpoint :

* Object detection : [job-object-detection-input.json](job-object-detection-input.json)
* Change detection : [job-change-detection-input.json](job-change-detection-input.json)
