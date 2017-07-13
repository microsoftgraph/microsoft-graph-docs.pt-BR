# Tipo de recurso plannerUserIds
<a id="planneruserids-resource-type" class="xliff"></a>

O recurso **plannerUserIds** representa a lista de ids de usuários com a qual um [plano](plannerplan.md) é compartilhado. Este é um Tipo Aberto. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.


## Propriedades
<a id="properties" class="xliff"></a>
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer identificações de usuário como propriedades e seus valores devem ser o booliano `true`. Quando as identificações de usuário já não forem compartilhadas, as propriedades serão automaticamente removidas ao configurar os valores com o booliano `false`.


## Representação JSON
<a id="json-representation" class="xliff"></a>

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

// Exemplo
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->