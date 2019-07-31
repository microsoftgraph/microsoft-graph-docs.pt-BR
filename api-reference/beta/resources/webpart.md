---
author: rahmit
description: O recurso webPart representa informações sobre o tipo e a renderização de uma Web Part em um sitePage.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007351"
---
# <a name="webpart-resource"></a>recurso webPart

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **WebPart** representa informações sobre o tipo e a renderização de uma Web Part em um [sitePage](sitepage.md).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo             | Descrição
|:------------------------|:-----------------|:----------------------------------
| **type**                | String           | Um identificador exclusivo que especifica o tipo de Web Part. Somente leitura.
| **data**                | [sitePageData][] | As propriedades necessárias para a Web Part (varia por webPart)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>Comentários

As Web Parts podem definir suas próprias propriedades obrigatórias em **Data**.

Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->
