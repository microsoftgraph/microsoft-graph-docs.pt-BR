---
title: tipo de recurso mentionsPreview
description: Representa informações sobre objetos de menção em uma instância de recurso.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523474"
---
# <a name="mentionspreview-resource-type"></a>tipo de recurso mentionsPreview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre objetos de [menção](../resources/mention.md) em uma instância de recurso.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| isMencionado | Booliano | True se o usuário conectado é mencionado na instância de recurso pai. Somente leitura. Oferece suporte a filtro. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionspreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
