# [oData](./odata.md)

## Services

### infos
 [GET v1.1/infos](https://sensorthings.umrsas.inrae.fr/test/v1.1/infos) ✔️

### Etat
 [GET v1.1/state](https://sensorthings.umrsas.inrae.fr/test/v1.1/state) ✔️
   
### Etats
 [GET v1.1/states](https://sensorthings.umrsas.inrae.fr/test/v1.1/states) ✔️

### Tous les servics disponibles
 [GET v1.1/Services](https://sensorthings.umrsas.inrae.fr/test/v1.1/Services) ✔️

### Etat d'un service
 [GET v1.1/Services(1)](https://sensorthings.umrsas.inrae.fr/test/v1.1/Services(1)) ✔️
 
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
