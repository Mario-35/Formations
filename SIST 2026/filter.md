# [oData](./odata.md)

## Filter

### eq
**GET** [/v1.1/Observations?$filter=result eq 310](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20eq%20310)

### ne
**GET** [/v1.1/Observations?$filter=result ne 45](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20ne%2045)

### gt
**GET** [/v1.1/Observations?$filter=result gt 90](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20gt%2090)

### gt AND lt
**GET** [/v1.1/Observations?$filter=result gt 20 and result lt 22](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20gt%2020%20and%20result%20lt%2022)

### ge
**GET** [/v1.1/Observations?$filter=result ge 90](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20ge%2090)

### lt
**GET** [/v1.1/Observations?$filter=result lt 90](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20lt%2090)

### le
**GET** [/v1.1/Observations?$filter=result le 90](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=result%20le%2090)

### and
**GET** [/v1.1/Things?$filter=name eq 'classic Thing' and description eq 'Description of classic Thing'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=name%20eq%20'classic%20Thing'%20and%20description%20eq%20'Description%20of%20classic%20Thing')

### or
**GET** [/v1.1/Things?$filter=name eq 'classic Thing' or description eq 'Description of Hack $debug=true Thing'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=name%20eq%20'classic%20Thing'%20or%20description%20eq%20'Description%20of%20Hack%20$debug=true%20Thing')


# Fonctions

### substringof
**GET** [/v1.1/Things?$filter=substringof('description', 'chamber') eq true](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=substringof('description',%20'chamber')%20eq%20true)

### substringof('name', 'with')
**GET** [/v1.1/Things?$filter=substringof('name', 'with')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=substringof('name',%20'with'))

### endwith
**GET** [/v1.1/Things?$filter=endswith('name', 'Thing') eq true](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=endswith('name',%20'Thing')%20eq%20true)

### endwith('description', 'one')
**GET** [/v1.1/Things?$filter=endswith('description', 'Thing')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=endswith('description',%20'Thing'))

### startswith
**GET** [/v1.1/Sensors?$filter=startswith('name', 'Hack') eq true](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Sensors?$filter=startswith('name',%20'Hack')%20eq%20true)

### endwith(description, 'one')
**GET** [/v1.1/Datastreams?$filter=startswith('name', 'Outlet')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Datastreams?$filter=startswith('name',%20'Outlet'))

### Length
**GET** [/v1.1/Things?$filter=length(description) le 25](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=length(description)%20le%2025)

### indexof
**GET** [/v1.1/Things?$filter=indexof('name', 'Piezo') eq 1](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=indexof('name',%20'Piezo')%20eq%201)

### substring(str, nb)
**GET** [/v1.1/Things?$filter=substring('name', 1) eq 'hing with new Location test'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=substring('name',%201)%20eq%20'hing%20with%20new%20Location%20test')

### substring(str, index, nb)
**GET** [/v1.1/Things?$filter=substring('description', 10, 6) eq 'outlet'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=substring('description',%2010,%206)%20eq%20'outlet')

### toLower
**GET** [/v1.1/Things?$filter=tolower('name') eq 'piezo f5b'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=tolower('name')%20eq%20'piezo%20f5b')

### toUpper
**GET** [/v1.1/Things?$filter=toupper('name') eq 'PIEZOMETER F4'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=toupper('name')%20eq%20'PIEZOMETER%20F4')

### trim
**GET** [/v1.1/Things?$filter=trim('name') eq 'Piezo F5b'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=trim('name')%20eq%20'Piezo%20F5b')

### concat[GET v1.1/Things?$filter=concat('name', 'test') eq 'Piezometer F4test'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Things?$filter=concat('name',%20'test')%20eq%20'Piezometer%20F4test')


# Dates

### Date
**GET** [/v1.1/Observations?$filter=resultTime eq 2017-01-13](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20eq%202017-01-13)

### search by resultTime eq 01-13-2017
**GET** [/v1.1/Observations?$filter=resultTime eq '13-01-2017'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20eq%20'13-01-2017')

### search by resultTime gt 13-01-2017
**GET** [/v1.1/Observations?$filter=resultTime gt '13-01-2017'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20gt%20'13-01-2017')

### search by resultTime lt 15-10-2021
**GET** [/v1.1/Observations?$filter=resultTime lt '15-10-2021'](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20lt%20'15-10-2021')

### Year
**GET** [/v1.1/Observations?$filter=year(resultTime) eq 2017](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=year(resultTime)%20eq%202017)

### Month
**GET** [/v1.1/Observations?$filter=month(resultTime) eq 2](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=month(resultTime)%20eq%202)

### Day
**GET** [/v1.1/Observations?$filter=day(resultTime) eq 5](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=day(resultTime)%20eq%205)

### Hour
**GET** [/v1.1/Observations?$filter=hour(resultTime) eq 12](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=hour(resultTime)%20eq%2012)

### minute
**GET** [/v1.1/Observations?$filter=minute(resultTime) eq 45](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=minute(resultTime)%20eq%2045)

### second
**GET** [/v1.1/Observations?$filter=second(resultTime) ge 40](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=second(resultTime)%20ge%2040)

### date
**GET** [/v1.1/Observations?$filter=date(resultTime) eq date(phenomenonTime)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=date(resultTime)%20eq%20date(phenomenonTime))

### time
**GET** [/v1.1/Observations?$filter=time(resultTime) ne time(phenomenonTime)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=time(resultTime)%20ne%20time(phenomenonTime))

### boundaries
**GET** [/v1.1/Observations?$filter=resultTime%20ge%202024-06-04%20and%20resultTime%20le%202024-06-05](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%2520ge%25202024-06-04%2520and%2520resultTime%2520le%25202024-06-05)

### Now()
**GET** [/v1.1/Observations?$filter=resultTime le now()](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=resultTime%20le%20now())


# Maths

### Observations Round
**GET** [/v1.1/Observations?$filter=round(result) eq 63](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=round(result)%20eq%2063)

### Observations Floor
**GET** [/v1.1/Observations?$filter=floor(result) eq 63](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=floor(result)%20eq%2063)

### Observations Ceiling
**GET** [/v1.1/Observations?$filter=ceiling(result) eq 63](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=ceiling(result)%20eq%2063)


# Geospatial

### Location Distance location
**GET** [/v1.1/Locations?$filter=geo.distance(location, geography'POINT(-1.6567440482485551 48.11256463781973)') lt 0.11](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Locations?$filter=geo.distance(location,%20geography'POINT(-1.6567440482485551%2048.11256463781973)')%20lt%200.11)
   
### FOI Distance Foi
**GET** [/v1.1/Observations?$filter=geo.distance(FeatureOfInterest/feature,geography'POINT(-4.108433416883344 47.99535576613954)') ge 1](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=geo.distance(FeatureOfInterest/feature,geography'POINT(-4.108433416883344%2047.99535576613954)')%20ge%201)

### Location Length location
**GET** [/v1.1/Locations?$filter=geo.length(location,'POINT(-1.6571736839366906 48.112731020713284)') lt 1](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Locations?$filter=geo.length(location,'POINT(-1.6571736839366906%2048.112731020713284)')%20lt%201)

### Location Length Foi
**GET** [/v1.1/Observations?$filter=geo.length(FeatureOfInterest/feature,'POINT(-1.6571736839366906 48.112731020713284)') lt 1](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=geo.length(FeatureOfInterest/feature,'POINT(-1.6571736839366906%2048.112731020713284)')%20lt%201)

### Location Intersects location
**GET** [/v1.1/Locations?$filter=geo.intersects(location,'LINESTRING(-1.6567440482485551 48.11256463781973, -4.108433416883344 47.99535576613954)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Locations?$filter=geo.intersects(location,'LINESTRING(-1.6567440482485551%2048.11256463781973,%20-4.108433416883344%2047.99535576613954)'))

### FOI Intersects Foi
**GET** [/v1.1/Observations?$filter=geo.intersects(FeatureOfInterest/feature, 'LINESTRING(-1.202481228298467 48.35475608212215, -4.108433416883344 47.99535576613954)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=geo.intersects(FeatureOfInterest/feature,%20'LINESTRING(-1.202481228298467%2048.35475608212215,%20-4.108433416883344%2047.99535576613954)'))

### Location Within location
**GET** [/v1.1/Locations?$filter=geo.within(location, geography'POINT(-4.108433416883344 47.99535576613954)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Locations?$filter=geo.within(location,%20geography'POINT(-4.108433416883344%2047.99535576613954)'))

### Location Within Foi
**GET** [/v1.1/Observations?$filter=geo.within(FeatureOfInterest/feature, geography'POINT(-1.202481228298467 48.354756082122154)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=geo.within(FeatureOfInterest/feature,%20geography'POINT(-1.202481228298467%2048.354756082122154)'))

### Location Disjoint location
**GET** [/v1.1/Locations?$filter=geo.disjoint(location,'MULTIPOINT(-3.377509239138959 47.74736066059859, -1.6567440482485551 48.11256463781973, -4.108433416883344 47.99535576613954)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Locations?$filter=geo.disjoint(location,'MULTIPOINT(-3.377509239138959%2047.74736066059859,%20-1.6567440482485551%2048.11256463781973,%20-4.108433416883344%2047.99535576613954)'))

### Location Disjoint Observations
**GET** [/v1.1/Observations?$filter=geo.disjoint(FeatureOfInterest/feature,'MULTIPOINT(-3.377509239138959 47.74736066059859, -1.6567440482485551 48.11256463781973, -4.108433416883344 47.99535576613954)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=geo.disjoint(FeatureOfInterest/feature,'MULTIPOINT(-3.377509239138959%2047.74736066059859,%20-1.6567440482485551%2048.11256463781973,%20-4.108433416883344%2047.99535576613954)'))

### Location Equals location
**GET** [/v1.1/Locations?$filter=geo.equals(location,'POINT(-3.377509239138959 47.74736066059859)')](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Locations?$filter=geo.equals(location,'POINT(-3.377509239138959%2047.74736066059859)'))

### Location Equals Foi
**GET** [/v1.1/Observations?$filter=geo.equals(FeatureOfInterest/feature,%27POINT(-1.202481228298467%2048.35475608212215)%27)](https://sensorthings.umrsas.inrae.fr/agrhys/v1.1/Observations?$filter=geo.equals(FeatureOfInterest/feature,%2527POINT(-1.202481228298467%252048.35475608212215)%2527))

