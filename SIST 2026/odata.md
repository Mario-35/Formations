# [STEAN](./index.md)

## Nous allons utiliser quelques requettes oData

## SOMAIRE

- [Basic](./basic.md)
- [CreateObservations](./CreateObservations.md)
- [Filter](./filter.md)
- [Services](./services.md)
- [Intervals](./intervals.md)



- [Créer un flux](./create.md)

## MODELE

![STA](../images/drawio_STA_V1.1.jpg "STA")



### Quelques exemples "complexes"

 [GET /test/v1.1/Things?$filter=Datastreams/ObservedProperty/description eq 'Description of classic Observed Property'](https://sensorthings.umrsas.inrae.fr/test/v1.1/Things?$filter=Datastreams/ObservedProperty/description%20eq%20'Description%20of%20classic%20Observed%20Property')

 [GET /test/v1.1/Observations?$filter=phenomenonTime gt 2024-06-05T02:15:01+02:00](https://sensorthings.umrsas.inrae.fr/test/v1.1/Observations?$filter=phenomenonTime%20gt%202024-06-05T02:15:01+02:00)

 [GET /test/v1.1/Things?$filter=Datastreams/unitOfMeasurement/name eq 'Pression'](https://sensorthings.umrsas.inrae.fr/test/v1.1/Things?$filter=Datastreams/unitOfMeasurement/name%20eq%20'Pression')

 [GET /test/v1.1/Things?$filter=Datastreams/unitOfMeasurement/name eq 'PM 2.5 Particulates (ug/m3)'](https://sensorthings.umrsas.inrae.fr/test/v1.1/Things?$filter=Datastreams/unitOfMeasurement/name%20eq%20'PM%202.5%20Particulates%20(ug/m3)')

 [GET /test/v1.1/Observations?$filter=result gt 290 or result eq 250](https://sensorthings.umrsas.inrae.fr/test/v1.1/Observations?$filter=result%20gt%20290%20or%20result%20eq%20250)

 [GET /test/v1.1/Observations?$filter=length(result) le 2](https://sensorthings.umrsas.inrae.fr/test/v1.1/Observations?$filter=length(result)%20le%202)

 [GET /test/v1.1/Datastreams?$filter=ObservedProperty/name eq 'stream level'](https://sensorthings.umrsas.inrae.fr/test/v1.1/Datastreams?$filter=ObservedProperty/name%20eq%20'stream%20level')

 [GET /test/v1.1/Things?$filter=Datastreams/Observations/resultTime ge 2020-06-01T00:00:00Z and Datastreams/Observations/resultTime le 2022-07-01T00:00:00Z](https://sensorthings.umrsas.inrae.fr/test/v1.1/Things?$filter=Datastreams/Observations/resultTime%20ge%202020-06-01T00:00:00Z%20and%20Datastreams/Observations/resultTime%20le%202022-07-01T00:00:00Z)



















 # Services

### infos
 [GET v1.1/infos](https://sensorthings.umrsas.inrae.fr/test/v1.1/infos)

### Etat
 [GET v1.1/state](https://sensorthings.umrsas.inrae.fr/test/v1.1/state)
   
### Etats
 [GET v1.1/states](https://sensorthings.umrsas.inrae.fr/test/v1.1/states)

### Tous les servics disponibles
 [GET v1.1/Services](https://sensorthings.umrsas.inrae.fr/test/v1.1/Services)

### Etat d'un service
 [GET v1.1/Services(1)](https://sensorthings.umrsas.inrae.fr/test/v1.1/Services(1))
 
### Création d'un service
### **Services**

```JSON
{
  "name": "SIST",
  "pg": {
    "host": "localhost",
    "port": 5432,
    "user": "SIST",
    "password": "SIST",
    "database": "SIST",
    "retry": 2
  },
  "version": "v1.1",
  "date_format": "DD/MM/YYYY hh:mi:ss",
  "nb_page": "200",
  "nb_graph": "1000000",
  "extensions": [
    "multiDatastream",
    "unique",
    "partitioned"
  ],
  "options": [
    "canDrop"
  ],
  "csvDelimiter": ";"
}
```

<form action="/traitement" method="post">
  <label for="nom">Nom :</label>
  <input type="text" id="nom" name="nom">
  
  <label for="email">E-mail :</label>
  <input type="email" id="email" name="email">
  
  <button type="submit">Envoyer</button>
</form> 