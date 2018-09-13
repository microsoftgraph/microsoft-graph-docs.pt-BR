# <a name="filesecuritystate-resource-type"></a>tipo de recurso fileSecurityState

Contém informações sobre o arquivo (não processo) relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|fileHash|[fileHash](filehash.md)|Tipo complexo contendo hashes de arquivo (criptográficos e sensíveis à localização).|
|name|Sequência de caracteres|Nome do arquivo (sem o caminho).|
|path|Sequência de caracteres|Caminho completo do arquivo/arquivo de imagem.|
|riskScore|Sequência de caracteres|Classificação de risco do arquivo de alerta gerada/calculada pelo provedor. Intervalo de valor recomendado de 0-1, que equivale a um percentual.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->