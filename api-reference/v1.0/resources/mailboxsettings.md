# <a name="mailboxsettings-resource-type"></a>Tipo de recurso mailboxSettings

Configurações para a caixa de correio principal do usuário conectado.


## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.|
|idioma|[localeInfo](localeinfo.md)|Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.|
|timeZone|string|O fuso horário padrão para a caixa de correio do usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->