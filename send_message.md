# send_message

Envoie un message à un utilisateur

```
POST /api/v1/send_message
```
- `token` - Jeton d’identification de l’utilisateur courant
- `userid` - Identifiant de l’utilisateur qui recevra le message
- `message` - Contenu du message à envoyer
- `key` - Clé de chiffrage utilisée

⚠️ Le contenu de `message` doit être chiffré en utilisant la clé publique de l'utilisateur à qui envoyer le message. `key` indique la clé qui à été utilisé. Si le message n'a pas été chiffré, alors `key` doit être à la valeur `0`.

Réponse :
```json
{
    "status" : "send",
    "messageId" : 94522585489,
    "sendDate" : "1675779959000"
}
```
`sendDate` est une date au format UTC