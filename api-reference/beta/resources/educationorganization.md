---
title: tipo de recurso educationOrganization
description: 'Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ae3add0c3541e1617fec6bb71f0e05bb8fdc1b3f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016678"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo   | Descrição                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| description    | String | Descrição da organização.                                                         |
| displayName    | String | Nome de exibição da organização.                                                        |
| externalSource | String | De onde esse usuário foi criado. Os valores possíveis são: `sis` , `lms` , ou `manual` . |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


