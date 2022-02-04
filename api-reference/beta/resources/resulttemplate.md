---
title: Tipo de recurso resultTemplate
description: 'Um dicionário de resultTemplateIds e valores associados, que incluem o nome e o esquema JSON dos modelos de resultado.'
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
---

# <a name="resulttemplate-resource-type"></a>Tipo de recurso resultTemplate

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um dicionário de **resultTemplateIds** e valores associados, que inclui o nome e o esquema JSON dos modelos de resultado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|key|String|ID de um modelo de resultado. Ele deve mapear para **um resultTemplateId** no [searchHit](searchhit.md).|
|displayName|String|Nome do modelo de resultado.|
|corpo|Json|Esquema JSON do modelo de resultado.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplate",
  "baseType": null
}-->


```json
{
   "resultTemplateId": {
      "displayName": "String",
      "body": "Json schema"
   }
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


