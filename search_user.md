# search_user

Recherche un utilisateur inscrit ayant un compte valide

```
GET /api/v1/search_user?q=username
```
- `q` - Nom de l’utilisateur (`username`) ou nom d'affichage (`displayName`)

Réponse :
```json
{
	"results" :{
        "userid" : 1,
        "displayName" : "Enzo Degraeve",
        "username" : "EnzoDeg40"
    },
    {
        "userid" : 2,
        "displayName" : "Léo Duff",
        "username" : "LeoDuffOff"
    }
}
```

⚠️ Le nombre de résultat est limité à 10 utilisateurs