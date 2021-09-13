---
title: tipo de recurso de site
description: Representa um site.
ms.localizationpriority: medium
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c0daa5106f70f049d070968749e5a7d391783d59
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134210"
---
# <a name="website-resource-type"></a>tipo de recurso de site

Namespace: microsoft.graph

Representa um site.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|type|websiteType| Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.|
|address|cadeia de caracteres|A URL do site.|
|displayName|cadeia de caracteres|O nome de exibição do site.|

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
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

