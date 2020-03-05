---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0e84f6d071423159918479bdb1836855fed113a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520868"
---
# <a name="sectionlinks-resource-type"></a>tipo de recurso sectionLinks

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Links para abrir uma seção do OneNote.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
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
|oneNoteClientUrl|[externalLink](externallink.md)|Abre a seção no cliente nativo do OneNote se ele estiver instalado.|
|oneNoteWebUrl|[externalLink](externallink.md)|Abre a seção no OneNote na Web.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
