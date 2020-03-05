---
author: rahmit
description: O recurso webPart representa informações sobre o tipo e a renderização de uma Web Part em um sitePage.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: efcf6aa1db31246af607cda85aa799fcc6804a34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519432"
---
# <a name="webpart-resource"></a>recurso webPart

Namespace: Microsoft. Graph

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
