# [oData](./odata.md)

## Dates

### Date
 [GET v1.1/Observations?$filter=resultTime eq 2017-01-13](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20eq%202017-01-13)

### search by resultTime eq 01-13-2017
 [GET v1.1/Observations?$filter=resultTime eq '13-01-2017'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20eq%20'13-01-2017')

### search by resultTime gt 13-01-2017
 [GET v1.1/Observations?$filter=resultTime gt '13-01-2017'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20gt%20'13-01-2017')

### search by resultTime lt 15-10-2021
 [GET v1.1/Observations?$filter=resultTime lt '15-10-2021'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20lt%20'15-10-2021')

### Year
 [GET v1.1/Observations?$filter=year(resultTime) eq 2017](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=year(resultTime)%20eq%202017)

### Month
 [GET v1.1/Observations?$filter=month(resultTime) eq 2](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=month(resultTime)%20eq%202)

### Day
 [GET v1.1/Observations?$filter=day(resultTime) eq 5](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=day(resultTime)%20eq%205)

### Hour
 [GET v1.1/Observations?$filter=hour(resultTime) eq 12](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=hour(resultTime)%20eq%2012)

### minute
 [GET v1.1/Observations?$filter=minute(resultTime) eq 45](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=minute(resultTime)%20eq%2045)

### second
 [GET v1.1/Observations?$filter=second(resultTime) ge 40](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=second(resultTime)%20ge%2040)

### date
 [GET v1.1/Observations?$filter=date(resultTime) eq date(phenomenonTime)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=date(resultTime)%20eq%20date(phenomenonTime))

### time
 [GET v1.1/Observations?$filter=time(resultTime) ne time(phenomenonTime)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=time(resultTime)%20ne%20time(phenomenonTime))

### boundaries
 [GET v1.1/Observations?$filter=resultTime%20ge%202024-06-04%20and%20resultTime%20le%202024-06-05](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%2520ge%25202024-06-04%2520and%2520resultTime%2520le%25202024-06-05)

### Now()
 [GET v1.1/Observations?$filter=resultTime le now()](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20le%20now())
