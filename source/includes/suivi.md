# Suivi de scolarité

## afficher mes notes
> pour y acceder :

```javascript
axios.get("/marks")
```
> format de reponse :

```json
[
   {
   "message":  "",
   "marks":"[marks]"
     
   }
]
```
Délivre les notes de l’étudiant faisant la recherche ainsi que les statistiques du groupe sur chacune d’entre elles.

`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
ETU

### HTTP Request

`GET /marks`

### URL Parameters
Parameter | Description
--------- | -----------



## afficher les notes d'un etudiant

##  
> pour y acceder :

```javascript
axios.get("/marks/455")
```
> format de reponse :

```json
[
   {
   "message":  "",
     
   }
]
```
Affiche les notes de l’étudiant concerné et les statistiques associées.



`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
SCO

### HTTP Request

`GET /marks/:id`

### URL Parameters
Parameter | Description
--------- | -----------
id| identifiant etudiant



## afficher mes competences
> pour y acceder :

```javascript
axios.get("/skills")
```
> format de reponse :

```json
[
   {
   "message":  "",
   "marks":"[skills]"
     
   }
]
```
Affiche l’avancée de l’étudiant dans chaque module et les compétences associées.


`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
ETU

### HTTP Request

`GET /skills`

### URL Parameters
Parameter | Description
--------- | -----------



## afficher les comptences d'un etudiant

##  
> pour y acceder :

```javascript
axios.get("/skills/455")
```
> format de reponse :

```json
[
   {
   "message":  "",
   "marks":"[skills]"
     
   }
]
```
Affiche l’avancée de l’étudiant concerné dans chaque module et les compétences associées.




`Authorization: token-user`

<aside class=notice>
Vous devez modifier le token
</aside>


### Access
SCO

### HTTP Request

`GET /skills/:id`

### URL Parameters
Parameter | Description
--------- | -----------
id| identifiant etudiant




