# <a name="cloudappsecuritystate-resource-type"></a>tipo de recurso cloudAppSecurityState

Contém informações com estado sobre o aplicativo na nuvem (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|destinationServiceIp|Cadeia de caracteres|Endereço IP de destino da conexão para o serviço/aplicativo em nuvem.|
|destinationServiceName|Cadeia de caracteres|Nome do serviço do aplicativo na nuvem (por exemplo "Equipe de vendas", "Recados", etc.).|
|riskScore|Cadeia de caracteres|Pontuação de risco calculada/gerada pelo provedor do aplicativo/serviço na nuvem. Intervalo de valor recomendado de 0-1, que equivale a um percentual.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->