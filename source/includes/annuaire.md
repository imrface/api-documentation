
# Annuaire



## affihcer contacts

> pour y acceder :

```javascript
axios.get("/contact")
```
Affiche le formulaire de recherche de contact


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
USI

### HTTP Request

`GET /contact`





## affihcer trombinoscope

> pour y acceder :

```javascript
axios.get("/trombi")
```
Affiche le trombinoscope


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
USI

### HTTP Request

`GET /trombi`







## rechercher

> pour y acceder :

```javascript
axios.get("/search")
```
Affiche les résultats de la requête




`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
USI

### HTTP Request

`GET /search`

### URL Parameters
Parameter | Description
--------- | -----------
q | les mots clés pour rechercher un contact



## affihcer un contact

> pour y acceder :

```javascript
axios.get("/contact/1")
```
Affiche le contact détaillé de l’utilisateur recherché


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
USI

### HTTP Request

`GET /contact/:id`

### URL Parameters
Parameter | Description
--------- | -----------
id | identifiant de l'utilisateur





## mettre à jour un contact

> pour y acceder :

```javascript
axios.put("/contact/1", values)
```
Permet de changer les informations de contact (ex: adr. perso, téléphone, adr. postale, …)


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
USI

### HTTP Request

`PUT /contact/:id`

### URL Parameters
Parameter | Description
--------- | -----------
id | identifiant de l'utilisateur
contact | données à mettre à jour



## ajouter un contact

> pour y acceder :

```javascript
axios.post("/contacts/admin", values)
```
> format de reponse :

```json
[
   {
   "id":"666" ,
   "message":  "utilsateur ajouté avec succés",
     
   }
]
```
Ajoute un nouvel utilisateur


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
SCO

### HTTP Request

`POST /contact/admin`

### URL Parameters
Parameter | Description
--------- | -----------
contact | données de nouvel utilsateur


## mettre à jour un contact

> pour y acceder :

```javascript
axios.put("/contacts/1/admin", values)
```
> format de reponse :

```json
[
   {
   "id":"666" ,
   "message":  "utilsateur modifié avec succés",
     
   }
]
```
Modifie la fiche contact d’un utilisateur


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
SCO

### HTTP Request

`PUT /contact/:id/admin`

### URL Parameters
Parameter | Description
--------- | -----------
id | identifiant de l'utilisateur
contact | données à mettre 



## supprimer un contact

> pour y acceder :

```javascript
axios.delete("/contacts/:id/admin", values)
```
> format de reponse :

```json
[
   {
   "message":  "utilsateur supprimé avec succés",
     
   }
]
```
Supprime la fiche contact de l’utilisateur


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
SCO

### HTTP Request

`DELETE /contact/:id/admin`

### URL Parameters
Parameter | Description
--------- | -----------
id | identifiant de l'utilisateur



