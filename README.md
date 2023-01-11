# STARGATE H2020 - GAIASENSE OGC SensorThings API 
OGC SensorThings API for Gaiasense data source in Stargate project.
Source data is modelled according to the Agriculture Information Model (AIM) and Stargate extensions .
Data is retrieved directly source REST API service, transformed on the fly. 

| :warning: Methods require 'application/json' in accept header, i.e., -H "accept: application/json"   |
|:-----------------------------------------------------------------------------------------------------|

## Table of Contents
- [ILIAD OGC SensorThings API](#iliad-ogc-sensorthings-api)
  - [Table of Contents](#table-of-contents)
  - [Base Resource Path](#base-resource-path)
  - [Observations](#observations)
    - [Retrieve all Observations](#retrieve-all-observations)
    - [Retrieve a specific Observation](#retrieve-a-specific-observation)
    - [Retrieve Datastream for a sepcific Observation](#retrieve-datastream-for-a-sepcific-observation)
    - [Retrieve FeatureOfInterest for a sepcific Observation](#retrieve-featureofinterest-for-a-sepcific-observation)
  - [Datastreams](#datastreams)
    - [Retrieve all the Datastreams](#retrieve-all-the-datastreams)
    - [Retrieve a specific Datastream.](#retrieve-a-specific-datastream)
    - [Retrieve all Observations related to the Datastream](#retrieve-all-observations-related-to-the-datastream)
    - [Retrieve ObservedProperty related to the Datastream](#retrieve-observedproperty-related-to-the-datastream)
    - [Retrieve Sensor related to the Datastream](#retrieve-sensor-related-to-the-datastream)
    - [Retrieve Thing related to the Datastream](#retrieve-thing-related-to-the-datastream)
  - [Features of Interest](#features-of-interest)
    - [Retrieve all FeaturesOfInterest](#retrieve-all-featuresofinterest)
    - [Retrieve a specific FeatureOfInterest](#retrieve-a-specific-featureofinterest)
    - [Retrieve all Observations related to a specific FeatureOfInterest](#retrieve-all-observations-related-to-a-specific-featureofinterest)
  - [Observed properties](#observed-properties)
    - [Retrieve all the Observed properties](#retrieve-all-the-observed-properties)
    - [Retrieve a specific ObservedProperty](#retrieve-a-specific-observedproperty)
    - [Retrieve all Datastreams related to a specific ObservedProperty](#retrieve-all-datastreams-related-to-a-specific-observedproperty)
  - [Sensors](#sensors)
    - [Retrieve all Sensors](#retrieve-all-sensors)
    - [Retrieve a specific Sensor](#retrieve-a-specific-sensor)
    - [Retrieve all Datastreams related to a specific Sensor](#retrieve-all-datastreams-related-to-a-specific-sensor)
  - [Things](#things)
    - [Retrieve all Things](#retrieve-all-things)
    - [Retrieve a specific Thing](#retrieve-a-specific-thing)
    - [Retrieve all Datastreams related to a specific Thing](#retrieve-all-datastreams-related-to-a-specific-thing)
    - [Retrieve all HistoricalLocations related to a specific Thing](#retrieve-all-historicallocations-related-to-a-specific-thing)
    - [Retrieve a Location of a specific Thing](#retrieve-a-location-of-a-specific-thing)
  - [Locations](#locations)
    - [Retrieve all Locations](#retrieve-all-locations)
    - [Retrieve a specific Location](#retrieve-a-specific-location)
    - [Retrieve all HistoricalLocations related to a specific Location](#retrieve-all-historicallocations-related-to-a-specific-location)
    - [Retrieve a Thing related to a specific Location](#retrieve-a-thing-related-to-a-specific-location)
  - [HistoricalLocations](#historicallocations)
    - [Retrieve all HistoricalLocations](#retrieve-all-historicallocations)
    - [Retrieve a specific HistoricalLocation](#retrieve-a-specific-historicallocation)
    - [Retrieve a Location for a specific HistoricalLocation](#retrieve-a-location-for-a-specific-historicallocation)
    - [Retrieve a Thing for a specific HistoricalLocation](#retrieve-a-thing-for-a-specific-historicallocation)


## Base Resource Path
```
https://w3id.org/iliad/api/v1.0
```
## Observations
### Retrieve all Observations
```
https://w3id.org/iliad/api/v1.0/Observations
```
### Retrieve a specific Observation
```
https://w3id.org/iliad/api/v1.0/Observations(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/Observations(4540-15-2078-Rhizostoma%20pulmo)
```
### Retrieve Datastream for a sepcific Observation
```
https://w3id.org/iliad/api/v1.0/Observations(id)/Datastream
```
For example:
```
https://w3id.org/iliad/api/v1.0/Observations(4540-15-2078-Rhizostoma%20pulmo)/Datastream
```
### Retrieve FeatureOfInterest for a sepcific Observation
```
https://w3id.org/iliad/api/v1.0/Observations(id)/FeatureOfInterest
```
For example:
```
https://w3id.org/iliad/api/v1.0/Observations(4540-15-2078-Rhizostoma%20pulmo)/FeatureOfInterest
```

## Datastreams
### Retrieve all the Datastreams
```
https://w3id.org/iliad/api/v1.0/Datastreams
```
### Retrieve a specific Datastream.
```
https://w3id.org/iliad/api/v1.0/Datastreams(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)
```
### Retrieve all Observations related to the Datastream
```
https://w3id.org/iliad/api/v1.0/Datastreams(id)/Observations
```
For example:
```
https://w3id.org/iliad/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)/Observations
```
### Retrieve ObservedProperty related to the Datastream
```
https://w3id.org/iliad/api/v1.0/Datastreams(id)/ObservedProperty
```
For example:
```
https://w3id.org/iliad/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)/ObservedProperty
```
### Retrieve Sensor related to the Datastream
```
https://w3id.org/iliad/api/v1.0/Datastreams(id)/Sensor
```
For example:
```
https://w3id.org/iliad/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)/Sensor
```
### Retrieve Thing related to the Datastream
```
https://w3id.org/iliad/api/v1.0/Datastreams(id)/Thing
```
For example:
```
https://w3id.org/iliad/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)/Thing
```


## Features of Interest
### Retrieve all FeaturesOfInterest
```
https://w3id.org/iliad/api/v1.0/FeaturesOfInterest
```
### Retrieve a specific FeatureOfInterest
```
https://w3id.org/iliad/api/v1.0/FeaturesOfInterest(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/FeaturesOfInterest(1-18)
```
### Retrieve all Observations related to a specific FeatureOfInterest
```
https://w3id.org/iliad/api/v1.0/FeaturesOfInterest(id)/Observations
```
For example:
```
https://w3id.org/iliad/api/v1.0/FeaturesOfInterest(1-18)/Observations
```

## Observed properties
### Retrieve all the Observed properties
```
https://w3id.org/iliad/api/v1.0/ObservedProperties
```
### Retrieve a specific ObservedProperty
```
https://w3id.org/iliad/api/v1.0/ObservedProperties(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/ObservedProperties(jellyFishAbundanceProperty)
```
### Retrieve all Datastreams related to a specific ObservedProperty
```
https://w3id.org/iliad/api/v1.0/ObservedProperties(id)/Datastreams
```
For example:
```
https://w3id.org/iliad/api/v1.0/ObservedProperties(jellyFishAbundanceProperty)/Datastreams
```

## Sensors
### Retrieve all Sensors
```
https://w3id.org/iliad/api/v1.0/Sensors
```
### Retrieve a specific Sensor
```
https://w3id.org/iliad/api/v1.0/Sensors(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/Sensors(1)
```
### Retrieve all Datastreams related to a specific Sensor
```
https://w3id.org/iliad/api/v1.0/Sensors(id)/Datastreams
```
For example:
```
https://w3id.org/iliad/api/v1.0/Sensors(1)/Datastreams
```

## Things
### Retrieve all Things
```
https://w3id.org/iliad/api/v1.0/Things
```
### Retrieve a specific Thing
```
https://w3id.org/iliad/api/v1.0/Things(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/Things(1)
```
### Retrieve all Datastreams related to a specific Thing
```
https://w3id.org/iliad/api/v1.0/Things(id)/Datastreams
```
For example:
```
https://w3id.org/iliad/api/v1.0/Things(2943)/Datastreams
```
### Retrieve all HistoricalLocations related to a specific Thing
```
https://w3id.org/iliad/api/v1.0/Things(id)/HistoricalLocations
```
For example:
```
https://w3id.org/iliad/api/v1.0/Things(2943)/HistoricalLocations
```
### Retrieve a Location of a specific Thing
```
https://w3id.org/iliad/api/v1.0/Things(id)/Locations
```
For example:
```
https://w3id.org/iliad/api/v1.0/Things(2943)/Locations
```

## Locations
### Retrieve all Locations
```
https://w3id.org/iliad/api/v1.0/Locations
```
### Retrieve a specific Location
```
https://w3id.org/iliad/api/v1.0/Locations(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/Locations(2943)
```
### Retrieve all HistoricalLocations related to a specific Location
```
https://w3id.org/iliad/api/v1.0/Locations(id)/HistoricalLocations
```
For example:
```
https://w3id.org/iliad/api/v1.0/Locations(2943)/HistoricalLocations
```
### Retrieve a Thing related to a specific Location
```
https://w3id.org/iliad/api/v1.0/Locations(id)/Things
```
For example:
```
https://w3id.org/iliad/api/v1.0/Locations(1)/Things
```

## HistoricalLocations
### Retrieve all HistoricalLocations
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations
```
### Retrieve a specific HistoricalLocation
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations(id)
```
For example:
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations(10089-3239)
```
### Retrieve a Location for a specific HistoricalLocation
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations(id)/Locations
```
For example:
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations(10089-3239)/Locations
```
### Retrieve a Thing for a specific HistoricalLocation
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations(id)/Things
```
For example:
```
https://w3id.org/iliad/api/v1.0/HistoricalLocations(10089-3239)/Things
```

For more information about OGC API please refer to:
* [GitHub repository](https://github.com/opengeospatial/sensorthings).
* [Test implementation](https://developers.sensorup.com/docs/#observations_get).

