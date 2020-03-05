---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fb7fea89a7da3d98899a19614d7c40f76dcb6f8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447644"
---
# <a name="itembody-resource-type"></a>Tipo de recurso itemBody

Namespace: Microsoft. Graph

Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|content|Cadeia de caracteres|O conteúdo do item.|
|contentType|BodyType|O tipo de conteúdo. Os valores possíveis são: `text` e `html`.|

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
