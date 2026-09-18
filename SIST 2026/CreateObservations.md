# [oData](./odata.md)

# CreateObservations

   213. Add datastream
 [POST v1.1/CreateObservations](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/CreateObservations)
```js
{
  "Datastream": { "@iot.id": 1 },
  "components": [ "phenomenonTime", "result", "resultTime", "FeatureOfInterest/id" ],
  "dataArray": [
    [ "2017-01-13T10:20:00.000Z", 90, "2017-01-13T10:20:00.000Z", 1, 4 ],
    [ "2017-01-13T10:21:00.000Z", 91, "2017-01-13T10:21:00.000Z", 1, 4 ],
    [ "2017-02-13T10:22:00.000Z", 92, "2017-02-13T10:22:00.000Z", 1, 4 ],
    [ "2017-02-13T10:23:00.000Z", 93, "2017-02-13T10:23:00.000Z", 1, 4 ]
  ]
}
```
