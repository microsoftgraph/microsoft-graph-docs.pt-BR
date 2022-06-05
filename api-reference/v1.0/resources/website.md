---
title: tipo de recurso do site
description: Representa um site.
ms.localizationpriority: medium
author: AAmatino
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: f63aba19d6f3e0e942ad35f445b43ed7b1bff1e3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899663"
---
# <a name="website-resource-type"></a>tipo de recurso do site

Namespace: microsoft.graph

Representa um site.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|type|Websitetype| Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.|
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

