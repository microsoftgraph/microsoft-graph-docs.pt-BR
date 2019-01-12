---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9147d434a94380c4d178efdf80ccba90734bf96f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939039"
---
# <a name="webpart-resource"></a>recurso de Web Part

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **Web Part** representa o tipo e informações de renderização de uma web part em um [sitePage](sitepage.md).

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo             | Descrição
|:------------------------|:-----------------|:----------------------------------
| **type**                | Cadeia de caracteres           | Um identificador exclusivo especificando o tipo de Web Part. Somente leitura.
| **data**                | [sitePageData][] | As propriedades necessárias para a Web Part (varia de acordo com a Web Part)

[sitePageData]: sitepagedata.md

## <a name="remarks"></a>Comentários

Web parts do podem definir suas próprias propriedades necessárias em **dados**.

Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
