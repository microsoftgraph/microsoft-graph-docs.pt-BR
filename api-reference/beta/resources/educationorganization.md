---
title: tipo de recurso educationOrganization
description: 'Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 015b1c886f439e3c5952d1c1a5fcce02fb21773b
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909650"
---
# <a name="educationorganization-resource-type"></a>tipo de recurso educationOrganization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade abstrata usada para modelar a semelhança entre diferentes tipos de organização dentro do setor educacional.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo   | Descrição                                                                       |
| :------------- | :----- | :-------------------------------------------------------------------------------- |
| description    | String | Descrição da organização.                                                         |
| displayName    | Cadeia de caracteres | Nome de exibição da organização.                                                        |
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
