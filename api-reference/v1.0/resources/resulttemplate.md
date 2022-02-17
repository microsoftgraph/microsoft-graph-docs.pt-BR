---
title: Tipo de recurso resultTemplate
description: Representa um dicionário de resultTemplateIds e valores associados, que incluem o nome e o esquema JSON dos modelos de resultado.
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f6c3583ce13da2bc1c94325ed4a7db7353f329f0
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62879261"
---
# <a name="resulttemplate-resource-type"></a>Tipo de recurso resultTemplate

Namespace: microsoft.graph

Representa um dicionário de **resultTemplateIds** e valores associados, que inclui o nome e o esquema JSON dos modelos de resultado.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|body|Json|Esquema JSON do modelo de resultado.|
|displayName|Cadeia de caracteres|Nome do modelo de resultado.|
|chave|Cadeia de caracteres|ID de um modelo de resultado. A **propriedade** key deve mapear para **um resultTemplateId** na [coleção searchHit](searchhit.md) .|

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
                        "body": {"@odata.type": "microsoft.graph.Json"}
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


