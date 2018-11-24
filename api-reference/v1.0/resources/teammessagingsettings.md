# <a name="teammessagingsettings-resource-type"></a>tipo de recurso de teamMessagingSettings



Configurações para configurar mensagens e menções na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowUserEditMessages|Booliano|Se definido como true, os usuários pode editar suas mensagens.|
|allowUserDeleteMessages|Booliano|Se definido como true, os usuários pode excluir suas mensagens.|
|allowOwnerDeleteMessages|Booliano|Se definido como true, proprietários pode excluir qualquer mensagem.|
|allowTeamMentions|Booliano|Se definido como true, @team menções são permitidas.|
|allowChannelMentions|Booliano|Se definido como true, @channel menções são permitidas.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
