# [oData](./odata.md)

## Nous allons utiliser quelques requettes oData

### All
 [GET v1.1/Things](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things)

### One
 [GET v1.1/Things(1)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things(1))

### Top
 [GET v1.1/Observations?$top=5](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$top=5)
   
### Skip
 [GET v1.1/Observations?$skip=500](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$skip=500)
   
### count
 [GET v1.1/Observations?$skip=3&$top=2&$count=true](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$skip=3&$top=2&$count=true) 

### Subentity
 [GET v1.1/Things(1)/Datastreams](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things(1)/Datastreams)
   
### Expand
 [GET v1.1/Things(6)?$expand=Datastreams](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things(1)?$expand=Datastreams)

### Select with Expand
 [GET v1.1/Things?$select=name,description&$expand=Datastreams](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$select=name,description&$expand=Datastreams)
    
### Expands
 [GET v1.1/Datastreams(9)?$expand=Observations,ObservedProperty](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Datastreams(9)?$expand=Observations,ObservedProperty)

### Select with Expand with inner select
 [GET v1.1/Things?$select=name,description&$expand=Datastreams($select=name)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$select=name,description&$expand=Datastreams($select=name))

### Only references
 [GET v1.1/Things/$ref](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1//Things/$ref)

### Nested resource path
 [GET v1.1/Things(6)/Datastreams(7)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things(6)/Datastreams(7))

### Filter nested resource path
 [GET v1.1/Things?$filter=Datastreams/description eq 'Pressure sensor'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=Datastreams/description%20eq%20'Pressure%20sensor')
  
### Complex filter nested resource path
 [GET v1.1/Things?$filter=Datastreams/ObservedProperty/description eq 'Mesure de la profondeur de la nappe'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=Datastreams/ObservedProperty/description%20eq%20'Mesure%20de%20la%20profondeur%20de%20la%20nappe')

### All datastream infos
 [GET v1.1/Datastreams(9)?$expand=Thing/Locations,Sensor,ObservedProperty](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Datastreams(9)?$expand=Thing/Locations,Sensor,ObservedProperty)

### From phenomenonTime search
 [GET v1.1/Datastreams?$filter=resultTime eq 2024-06-01T03:00:01Z/2024-06-03T03:45:01Z](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Datastreams?$filter=resultTime%20eq%202024-06-01T03:00:01Z/2024-06-03T03:45:01Z)

### Multi Select
 [GET v1.1/Observations(1)?$select=phenomenonTime,result](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations(1)?$select=phenomenonTime,result)
 

