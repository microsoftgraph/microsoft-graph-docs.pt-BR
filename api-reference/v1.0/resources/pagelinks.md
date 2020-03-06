---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dd6f5405f419561a2ec7587fab8f36245947f257
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534090"
---
# <a name="pagelinks-resource-type"></a>tipo de recurso pageLinks

Namespace: microsoft.graph

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
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
