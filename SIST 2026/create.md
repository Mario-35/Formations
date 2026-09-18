# [oData](./odata.md)

## Nous allons créer un flux de donnée

### **Thing**
```JSON
{
  "name": "Atelier SIST 2026",
  "description": "Example atelier SIST 2026",
  "properties": {
    "image": "https://sist.cnrs.fr/wp-content/uploads/2024/02/cropped-SIST-sans-texte-l200.png"
  }
}
```

### **Location**
```JSON
{
  "name": "Maison des Sciences",
  "description": "Maison des Sciences de Dijon",
  "encodingType": "application/geo+json",
  "location": {
    "type": "Point",
    "coordinates": [
      47.312752304764594,
      5.064659215341594
    ]
  }
}
```

### **Sensor**
```JSON
{
  "name": "Capteur quelconque",
  "description": "Capteur de niveau de quelquechose",
  "encodingType": "application/pdf",
  "metadata": "https://sensorthings.umrsas.inrae.fr/public/sensors/metadonneeshQ20250326.pdf",
  "properties": {
    "maxValue": "",
    "minValue": ""
  }
}
```

### **ObservedProperty**
```JSON
{
  "name": "Niveau mesuré",
  "description": "Mesure de niveau de liquide",
  "definition": "https://w3id.org/ozcar-theia/c_158149bf",
  "properties": {
    "theme": "hydrology",
    "unit-name": "Meter",
    "unit-symbol": "m",
    "skos:broader": "",
    "theme/category": "",
    "unit-definition": "http://qudt.org/vocab/unit/M"
  }
}
```

### **Datastream**

```JSON
{
  "name": "Mesure du bidule",
  "description": "Flux de données du bidule en mètre",
  "observationType": "http://www.opengis.net/def/observationType/OGC-OM/2.0/OM_Measurement",
  "unitOfMeasurement": {
    "name": "Meter",
    "symbol": "m",
    "definition": "http://qudt.org/vocab/unit/M"
  },
  "Thing": {
    "@iot.name": "Atelier SIST 2026"
  },
  "Location": {
    "@iot.name": "Maison des Sciences"
  },
  "Sensor": {
    "@iot.name": "Capteur quelconque"
  },
  "ObservedProperty": {
    "@iot.name": "Niveau mesuré"
  }
}
```

### La même chose en une opération

### **Thing**
```JSON
{
  "name": "Atelier SIST 2026",
  "description": "Example atelier SIST 2026",
  "properties": {
    "image": "https://sist.cnrs.fr/wp-content/uploads/2024/02/cropped-SIST-sans-texte-l200.png"
  },
  "Locations": [
    {
      "name": "Maison des Sciences",
      "description": "Maison des Sciences de Dijon",
      "encodingType": "application/geo+json",
      "location": {
        "type": "Point",
        "coordinates": [
          47.312752304764594,
          5.064659215341594
        ]
      }
    }
  ],
  "Datastreams": [
    {
      "name": "Mesure du bidule",
      "description": "Flux de données du bidule en mètre",
      "observationType": "http://www.opengis.net/def/observationType/OGC-OM/2.0/OM_Measurement",
      "unitOfMeasurement": {
        "name": "Meter",
        "symbol": "m",
        "definition": "http://qudt.org/vocab/unit/M"
      },
      "ObservedProperty": {
        "name": "Niveau mesuré",
        "description": "Mesure de niveau de liquide",
        "definition": "https://w3id.org/ozcar-theia/c_158149bf",
        "properties": {
          "theme": "hydrology",
          "unit-name": "Meter",
          "unit-symbol": "m",
          "skos:broader": "",
          "theme/category": "",
          "unit-definition": "http://qudt.org/vocab/unit/M"
        }
      },
      "Sensor": {
        "name": "Capteur quelconque",
        "description": "Capteur de niveau de quelquechose",
        "encodingType": "application/pdf",
        "metadata": "https://sensorthings.umrsas.inrae.fr/public/sensors/metadonneeshQ20250326.pdf",
        "properties": {
          "maxValue": "",
          "minValue": ""
        }
      }
    }
  ]
}
```
