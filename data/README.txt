
## This file shows how the data is structured.

Each file represents a state.
They must be formatted in JSON.

The name of the file must be an ID of a state. Following are the ID's of the states:

MX-AGU
MX-BCN
MX-BCS
MX-CAM
MX-CHP
MX-CHH
MX-COA
MX-COL
MX-DF 
MX-DUR
MX-GUA
MX-GRO
MX-HID
MX-JAL
MX-MEX
MX-MIC
MX-MOR
MX-NA 
MX-NLE
MX-OAX
MX-PUE
MX-QUE
MX-ROO
MX-SLP
MX-SIN
MX-SON
MX-TAB
MX-TAM
MX-TLA
MX-VER
MX-YUC
MX-ZAC

### JSON structure

The file must have an object *equipos* with an array of objects representing the teams. 
Such objects must have the name (*nombre*) of the team and a details (*detalles*) list.
Withing the details, any pair of key value can be added.

´´´
{
    "equipos": [        
        {
            "nombre": "Mi equipo",
            "detalles": {
                "Entrenador":"Casds Oodfo",
                "email":"miequipo@ejemplo.com"
            }
        }       
    ]
}
´´´

### Special handling

Some keys are shown in a different way, i.e. if there is a key *Facebook*, the page will show a facebook
logo with a link to the specified URL.

Below are the keys with special handling:

- **Facebook** : The result is a facebook logo with a link to the specified URL. The value must be a URL. 
- **Logo** : The value must be the path of a image. This image will be shown at the team thumbnail.

