---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
localization_priority: Normal
ms.openlocfilehash: f7293b986b5e6d77d0601cffb6b60edc5dfd2dd7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856025"
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
