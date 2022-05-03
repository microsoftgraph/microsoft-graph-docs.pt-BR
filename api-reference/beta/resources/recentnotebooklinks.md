---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um OneNote bloco de anotações. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: notes
author: jewan-microsoft
ms.openlocfilehash: bb9b7836569ed040a1b2f5c14b7e4a4ed458b983
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176879"
---
# <a name="recentnotebooklinks-resource-type"></a>tipo de recurso recentNotebookLinks

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Links para abrir um OneNote bloco de anotações. Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Abre o notebook no OneNote cliente, se ele estiver instalado.|
|oneNoteWebUrl|[externalLink](externallink.md)|Abre o bloco de anotações OneNote na Web.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


