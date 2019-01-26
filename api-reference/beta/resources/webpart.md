---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e7bbd0f6aa8d4ea04304d6aecae97b98ab0a46b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574275"
---
# <a name="webpart-resource"></a>recurso de Web Part

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso de **Web Part** representa o tipo e informações de renderização de uma web part em um [sitePage](sitepage.md).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  
    ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "String (identifier)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo             | Descrição
|:------------------------|:-----------------|:----------------------------------
| **type**                | Cadeia de caracteres (identificador)         | Um identificador exclusivo especificando o tipo de Web Part. Somente leitura.
| **data**                | [sitePageData](sitepagedata.md) | As propriedades necessárias para a Web Part (varia de acordo com a Web Part)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>Comentários

Web parts do podem definir suas próprias propriedades necessárias em **dados**.

Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
