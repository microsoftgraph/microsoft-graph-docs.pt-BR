# <a name="onpremisesprovisioningerror-resource-type"></a>tipo de recurso onPremisesProvisioningError

Representa os erros de sincronização de diretório para as entidades de [usuário](user.md) e [grupo](group.md) quando durante a sincronização local de diretórios no Active Directory do Azure.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
|category|Sequência de caracteres| Categoria do erro de configuração. Observação: No momento, há apenas um valor possível. Valor possível: *PropertyConflict* - indica que o valor de uma propriedade não é único. Outros objetos contêm o mesmo valor para a propriedade. |
|occurredDateTime|DateTimeOffset| A data e hora em que o erro ocorreu. |
|propertyCausingError|Sequência de caracteres| Nome da propriedade de diretório que causou o erro. Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress* |
|value|Sequência de caracteres| Valor da propriedade que causou o erro. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->