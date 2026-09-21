# [STEAN](./index.md)

## Exportation :

STEAN offre la possibilité d’exporter en csv en utilisant la puissance de PostgreSQL et de la fonction COPY. Une mécanique de streaming csv a été développée afin de pouvoir importer de grande masse de csv sans avoir à le stocker sur le serveur de façon très rapide et ce sans limite de taille.

http://rootApi/export 

Cette fonctionnalité permet d'exporter une structure complete (sans les observations) au format JSON

En y renseignant un nom, une database, password different et correct si vous effectuez un **POST** de ce JSON dans l'entité Services vous recréer totalement ce service sans les observations (mais vous pouvez pas l'import puis export csv le faire).