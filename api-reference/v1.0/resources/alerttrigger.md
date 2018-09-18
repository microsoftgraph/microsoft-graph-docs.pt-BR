# <a name="alerttrigger-resource-type"></a>Tipo de recurso alertTrigger

Contém informações sobre as propriedades que dispararam uma detecção (as propriedades existem na entidade alerta).

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|name|Sequência de caracteres|Nome da propriedade servindo como um disparo de detecção.|
|type|Sequência de caracteres|Tipo da propriedade no par de chave:valor para interpretação. Por exemplo, sequência de caracteres, Booleano, etc.|
|value|Sequência de caracteres|Nome da propriedade que serve como um disparo de detecção.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a>Exemplo

```json
{
  "name": "endpointAddress",
  "type": "networkConnection.sourceAddress",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->