# STARGATE H2020 - GAIASENSE OGC SensorThings API 
OGC SensorThings API for Gaiasense data source in Stargate project.
Source data is modelled according to the Agriculture Information Model (AIM) and Stargate extensions .
Data is retrieved directly source REST API service, transformed on the fly. 

| :warning: Methods require 'application/json' in accept header, i.e., -H "accept: application/json"   |
|:-----------------------------------------------------------------------------------------------------|

## Table of Contents
- [Base Resource Path](#Base-Resource-Path)
- [Observations](#Observations)
  * [Retrieve all Observations](#Retrieve-all-Observations)
  * [Retrieve a specific Observation](#Retrieve-a-specific-Observation)
  * [Retrieve Observations for a specific Datastream](#Retrieve-Observations-for-a-specific-Datastream)
- [Datastreams](#Datastreams)
  * [Retrieve all Datastreams](#Retrieve-all-Datastreams)
  * [Retrieve a specific Datastream](#Retrieve-a-specific-Datastream)
  * [Retrieve Datastream for a specific Observation](#Retrieve-Datastream-for-a-specific-Observation)
- [Features of Interest](#Features-of-Interest)
  * [Retrieve all FeaturesOfInterest](#Retrieve-all-FeaturesOfInterest)
  * [Retrieve a specific FeatureOfInterest](#Retrieve-a-specific-FeatureOfInterest)
  * [Retrieve FeatureOfInterest for a specific Observation](#Retrieve-FeatureOfInterest-for-a-specific-Observation)
- [Observed properties](#Observed-properties)
  * [Retrieve all the Observed properties](#Retrieve-all-the-Observed-properties)
  * [Retrieve the ObservedProperty of a specific Datastream.](#Retrieve-the-ObservedProperty-of-a-specific-Datastream.)
- [Sensors](#Sensors)
  * [Retrieve all Sensors](#Retrieve-all-Sensors)
  * [Retrieve a specific Sensor](#Retrieve-a-specific-Sensor)
  * [Retrieve the Sensor of a specific Datastream](#Retrieve-the-Sensor-of-a-specific-Datastream)
- [Things](#Things)
  * [Retrieve all Things](#Retrieve-all-Things)
  * [Retrieve a specific Thing](#Retrieve-a-specific-Thing)
  * [Retrieve the Thing of a specific Datastream](#Retrieve-the-Thing-of-a-specific-Datastream)


## Base Resource Path
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0
```
## Observations
### Retrieve all Observations
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Observations
```
### Retrieve a specific Observation
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Observations(id)
```
For example:
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Observations(3-10-361-Rhopilema%2520nomadica)
```
### Retrieve Observations for a specific Datastream
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0//Datastreams(id)/Observations
```
For example:
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)/Observations
```

## Datastreams
### Retrieve all the Datastreams
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Datastreams
```
### Retrieve a specific Datastream.
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Datastreams(id)
```
For example:
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Datastreams(3-jellyFishAbundanceProperty)
```
### Retrieve DataStream for a specific Observation
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Observations(id)/Datastream
```


## Features of Interest
### Retrieve all FeaturesOfInterest

### Retrieve a specific FeatureOfInterest

### Retrieve FeatureOfInterest for a specific Observation
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0/Observations(id)/FeatureOfInterest
```

## Observed properties
### Retrieve all the Observed properties

### Retrieve the ObservedProperty of a specific Datastream.
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0//Datastreams(id)/ObservedProperty
```

## Sensors
### Retrieve all Sensors

### Retrieve a specific Sensor

### Retrieve the Sensor of a specific Datastream
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0//Datastreams(id)/Sensor
```

## Things
### Retrieve all Things

### Retrieve a specific Thing

### Retrieve the Thing of a specific Datastream
```
https://w3id.org/stargate-h2020/gaiasense/api/v1.0//Datastreams(id)/Thing
```


For more information about OGC API please refer to:
* [GitHub repository](https://github.com/opengeospatial/sensorthings).
* [Test implementation](https://developers.sensorup.com/docs/#observations_get).

