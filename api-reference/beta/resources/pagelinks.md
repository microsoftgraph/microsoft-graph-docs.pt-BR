---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 3442862f52c1d8f6dd29ea2a2a0e99b2f65970f0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812524"
---
# <a name="pagelinks-resource-type"></a>tipo de recurso pageLinks

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Links para abrir uma página do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Abre a página no cliente nativo do OneNote se ele estiver instalado.|
|oneNoteWebUrl|[externalLink](externallink.md)|Abre a página no OneNote na Web.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
