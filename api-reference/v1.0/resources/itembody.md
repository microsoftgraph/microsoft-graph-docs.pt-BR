---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 44c48b916a625ce00a30474583fa45b2c1d37e3d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084304"
---
# <a name="itembody-resource-type"></a>Tipo de recurso itemBody

Namespace: microsoft.graph

Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|content|Cadeia de caracteres|O conteúdo do item.|
|contentType|bodyType|O tipo de conteúdo. Os valores possíveis são: `text` e `html`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

