# Mission 0 :

## BRUNO : 
<p align="center">
  <img src="./Pasted-image-20260908092111.png" width="100%">
</p>
<p align="center">
  <img src="./Pasted-image-20260908093151.png" width="100%">
</p>

## POSTMAN :
<p align="center">
  <img src="./Pasted-image-20260908092248.png" width="100%">
</p>
<p align="center">
  <img src="./Pasted-image-20260908092853.png" width="100%">
</p>

# Mission 1 :

## Étape 1 – Première requête GET

Pour la première étape, j’ai utilisé la méthode **GET**.

J’ai envoyé une requête vers :

`172.16.3.254:8001/bienvenue`

Cette étape m’a permis de comprendre le fonctionnement d’une requête HTTP simple. Je n’avais aucun paramètre ni donnée supplémentaire à envoyer.

Pour réussir cette étape, j’ai donc sélectionné la méthode **GET**, renseigné l’URL demandée puis envoyé la requête avec Bruno.

---

## Étape 2 – Utilisation d’un paramètre

Pour la deuxième étape, j’ai de nouveau utilisé la méthode **GET**, mais cette fois avec un paramètre dans l’URL.

L’adresse utilisée était :

`172.16.3.254:8001/decouverte-des-parametres?nom=Ethan`

J’ai ajouté le paramètre :

* `nom = Ethan`

Cette étape m’a permis de découvrir les **paramètres de requête**, également appelés *query parameters*.

Pour réussir l’étape, j’ai ajouté le paramètre `nom` avec la valeur `Ethan` dans Bruno. Celui-ci est ensuite apparu dans l’URL après le symbole `?`.

---

## Étape 3 – Utilisation de plusieurs paramètres

Pour cette étape, j’ai toujours utilisé une requête **GET**, mais avec plusieurs paramètres.

L’URL était :

`172.16.3.254:8001/plusieurs-parametres?prenom=Ethan&age=19`

J’ai utilisé deux paramètres :

* `prenom = Ethan`
* `age = 19`

J’ai appris qu’il est possible d’envoyer plusieurs paramètres dans une même requête. Le premier commence après le symbole `?` et les paramètres suivants sont séparés avec le symbole `&`.

Pour réussir cette étape, j’ai donc correctement renseigné les deux paramètres dans Bruno avant d’envoyer ma requête.

---

## Étape 4 – Découverte de la méthode POST

Pour la quatrième étape, j’ai utilisé pour la première fois la méthode **POST**.

La requête était envoyée vers :

`172.16.3.254:8001/un-peu-de-post`

Contrairement à GET, la méthode POST sert généralement à envoyer ou créer des données sur un serveur.

Pour réussir cette étape, j’ai remplacé la méthode GET par **POST**, renseigné la bonne URL puis envoyé la requête.

---

## Étape 5 – Utilisation du Content-Type

Pour cette étape, j’ai utilisé une requête **POST** vers :

`172.16.3.254:8001/5-content-type`

J’ai également ajouté un en-tête HTTP :

`Content-Type: application/json`

Le `Content-Type` permet d'indiquer au serveur le format des données envoyées. Ici, j’ai précisé que le contenu était au format **JSON**.

Pour réussir cette étape, j’ai donc ajouté l’en-tête `Content-Type` dans la partie **Headers** de Bruno avec la valeur `application/json`.

---

## Étape 6 – Utilisation de PUT et des Headers

Pour la sixième étape, j’ai découvert la méthode **PUT**.

J’ai envoyé la requête vers :

`172.16.3.254:8001/put-method-6`

J’ai également utilisé deux en-têtes HTTP :

* `Content-Type: text/html`
* `Accept: application/json`

Le `Content-Type` précise le format des données envoyées au serveur, tandis que `Accept` permet de préciser le format de réponse que je souhaite recevoir.

Dans cette étape, j’indique donc que le contenu envoyé est de type **HTML**, mais que je souhaite recevoir une réponse au format **JSON**.

Pour réussir l’étape, j’ai sélectionné la méthode PUT et ajouté correctement les deux Headers demandés.

---

## Étape 7 – Utilisation de DELETE

Pour cette étape, j’ai découvert la méthode **DELETE**.

L’URL utilisée était :

`172.16.3.254:8001/et-oui-delete?filename=bonjour`

J’ai ajouté le paramètre :

* `filename = bonjour`

La méthode DELETE est utilisée pour demander la suppression d’une ressource.

Ici, le paramètre `filename` permet d’indiquer au serveur quelle ressource est concernée par la suppression.

Pour réussir cette étape, j’ai sélectionné la méthode **DELETE**, renseigné le paramètre `filename` avec la valeur `bonjour`, puis envoyé la requête.

---

## Étape 8 – Utilisation de PATCH et d’un Body JSON

Pour la huitième étape, j’ai utilisé la méthode **PATCH**.

La requête était envoyée vers :

`172.16.3.254:8001/etape8/api/users/12345`

J’ai ajouté l’en-tête :

`Content-Type: application/json`

J’ai également ajouté un **Body au format JSON** contenant :

```json
{
  "role": "Developer",
  "email": "blablabla@gmail.com"
}
```

Cette étape m’a permis d’apprendre à envoyer des données directement dans le corps d’une requête.

La méthode PATCH sert généralement à modifier seulement certaines informations d’une ressource existante. Ici, la ressource concernée est l’utilisateur ayant l’identifiant `12345`.

Pour réussir cette étape, j’ai sélectionné PATCH, choisi un Body au format JSON et renseigné correctement les champs `role` et `email`.

---

## Étape 9 – Requête POST avec plusieurs Headers

Pour la dernière étape, j’ai utilisé une requête **POST** vers :

`172.16.3.254:8001/etape9`

Cette étape était plus complète car j’ai dû utiliser plusieurs Headers :

* `Content-Type: application/json`
* `api-key: FenelonBTSSIO`
* `User-Agent: FenelonBTSSIO-UserAgent-LaRochelle-v1.0`

J’ai également envoyé un Body JSON :

```json
{
  "name": "Donald Duck"
}
```

Le `Content-Type` indique encore une fois que les données sont envoyées au format JSON.

L’`api-key` correspond à une clé permettant au serveur d’identifier ou d’autoriser la requête.

Le `User-Agent` permet d’identifier le client qui envoie la requête.

Pour réussir cette dernière étape, j’ai donc dû faire attention à trois éléments : utiliser la bonne méthode POST, ajouter les trois Headers demandés et envoyer le Body au bon format JSON.

Ce TP m’a donc permis de mieux comprendre comment un client peut communiquer avec un serveur grâce au protocole HTTP et comment les API utilisent les méthodes, les paramètres, les Headers et les données JSON.
