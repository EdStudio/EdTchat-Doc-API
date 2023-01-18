## auth

S'identifie au serveur

```
POST /api/v1/auth
```

Solution 1 :
- `username` - Nom d'utilisateur
- `password` - Mot de passe

Solution 2 :
- `userid` - Identifiant de l'utilisateur
- `refreshToken` - Jeton de rafraichissement

Réponse : 
```json
{
    "token": "3*ZfTBap...",
    "validity": "1675779959000",
    "refreshToken" : "zZ0#tRKb..." 
}
```

