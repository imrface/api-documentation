# emploi du temps

## planning
> pour y acceder :

```javascript
axios.get("/planning")
```
> format de reponse :

```json
[
   {
   "message":  "",
     
   }
]
```
Affichage de l’emploi du temps de la personne en faisant la recherche


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
CRS

### HTTP Request

`GET /planning`

### URL Parameters
Parameter | Description
--------- | -----------





##  recherche planning
> pour y acceder :

```javascript
axios.get("/planning/imr1/2021")
```
> format de reponse :

```json
[
   {
   "message":  "",
     
   }
]
```
Affichage de l’emploi du temps du groupe concerné par la recherche



`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
CRSCRS,
RP,
SEC, 
DDE,
DIR, 
TAC

### HTTP Request

`GET /planning/:q/:year`

### URL Parameters
Parameter | Description
--------- | -----------
q | promotion
year | l'année



