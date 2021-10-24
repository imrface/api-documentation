# Introduction

Bienvenu INSSAT API! 


Cette documentation est réalisé au fur et à mesure de notre avancent pendant le projet,
il va nous permettre de simplifier la communication entre notre back-end et front-end, surtout la methode http, paramatres, fromat de reponses

# Liste des utilisateurs

## codes de utilisateurs
Code | sens 
--------- | ------- 
AE	|Diplômés (ancien étudiant)
DIR	|	Directeur de l’établissement
DDE	|	Direction des études
ENS	|	Enseignants
ETU	|	Étudiants
CAN	|	Candidat
GRE	|	Gestionnaires relations entreprise
GRH	|	Gestionnaire ressources humaines
SCO	|	Gestionnaires scolarité
MA	|	Maître d’apprentissage
MS	|	Maître de stage
RP	|	Responsables pédagogiques
DOC	|	Doctorant
VAC	|	Vacataire
TAC	|	Tuteur académique
BU	|	Responsable de la bibliothèque universitaire
PAC	|	Partenaire académique
TEC	|	Equipe technique
INT	|	Intranet (Système)
<aside class=success>
une lsite des utilsateurs 
</aside>

## codes de Groupes

Code | sens  | membres
--------- | ------- | ------- 
ADM	|	Administration |	{GRE, GRH, SCO, DIR}
USA	|	Utilisateur	|Ω \ {INT}
USI	|	Utilisateur interne |	{ETU, ENS, DDE, GRE, GRH, SCO, DIR, RP, VAC, TAC, TEC, DOC, BU}
USE	|	Utilisateur externe|	{AE, CAN, MA, MS, PAC}
CRS	|	Personnes disposant de cours sur l’emploi du temps	| {ENS, VAC, ETU, DOC}
SEC	|	Secrétariat |	{SCO, GRH}
<aside class=success>
liste de groupe
</aside>


## Enumérations
### application_status
Label |
--------- | 
application|
eligible|
accepted|

# Authentication

## login

> Pour se connecter , vous utilisez ce code:


```javascript
import axios from 'axios';

const response = axios.post("login", values);
```



> Le format json de cette requette http:

```json
[
   {
      "id":         1,
      "profil":       "Fluffums",
      "token":      "FGHJKL78999"
   }
]
```


Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

### HTTP Request

`POST http://localhost:8000/login`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of user
Passowrd | The passowrd of user

<aside class=notice>
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

## logout

> Pour se connecter , vous utilisez ce code:


```javascript
import axios from 'axios';

const response = axios.get("logout");
```



> Le format json de cette requette http:

```json
[
   {
   
      "message":       "disconnected success",
     
   }
]
```

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

### HTTP Request (with ID)

`POST http://localhost:8000/logout`

### URL Parameters

aucun paramtre

<aside class=notice>
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>
