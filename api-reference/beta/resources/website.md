---
title: tipo de recurso site
description: Representa um site da Web.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 4c283d77119c0272aaafa964db62bb35ad747a10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973467"
---
# <a name="website-resource-type"></a>tipo de recurso site

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um site da Web.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|tipo|String| Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.|
|address|cadeia de caracteres|A URL do site.|
|displayName|string|O nome de exibição do site da Web.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


