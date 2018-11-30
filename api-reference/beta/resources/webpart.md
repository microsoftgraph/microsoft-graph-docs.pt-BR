---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036140"
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
| **type**                | String           | Um identificador exclusivo especificando o tipo de Web Part. Somente leitura.
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
