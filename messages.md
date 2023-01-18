# messages

Récupère les derniers des messages venant d'une conversation avec un autre utilisateur

```
GET /api/v1/get_messages
```

- `token` - Jeton d’identification de l’utilisateur courant
- `userid` - Identifiant de l’utilisateur avec qui la conversation est établie
- `number` - Nombre de messages à récupérer (par défaut 10, maximum 50)
- `before` - Récupère les messages envoyés avant la date spécifiée (par défaut la date actuelle)

Réponse :

```json
{
    "messages" : [
        {
            "messageId" : 94522585489,
            "senderId" : 1,
            "receiverId" : 2,
            "message" : "Hello",
            "key" : 0,
            "sendDate" : "1675779959000"
        },
        {
            "messageId" : 94522585490,
            "senderId" : 2,
            "receiverId" : 1,
            "message" : "Hello",
            "key" : 0,
            "sendDate" : "1675779959000"
        }
    ]
}
```