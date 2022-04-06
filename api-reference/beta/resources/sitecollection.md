---
author: JeremyKelley
description: O recurso siteCollection fornece mais informações sobre um conjunto de sites.
ms.date: 09/10/2017
title: SiteCollection
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1a2d685382eb96d332408a0f03131b5ab0cd6d02
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720821"
---
# <a name="sitecollection-resource"></a>Recurso SiteCollection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.

Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo     | Descrição                                                                         |
| :------------------- | :------- | :---------------------------------------------------------------------------------- |
| **hostname**         | string   | O nome do host do conjunto de sites. Somente leitura.                                    |
| **dataLocationCode** | string   | O código de região geográfica para onde esse conjunto de sites reside. Somente leitura.       |
| **root**             | [root][] | Se presente, indica que esse é um conjunto de sites raiz no SharePoint. Somente leitura. |

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
