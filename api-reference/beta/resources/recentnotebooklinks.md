---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f98feb5e9fbe5cede591f4edf0349b3bf4267de9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521254"
---
# <a name="recentnotebooklinks-resource-type"></a>tipo de recurso recentNotebookLinks

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.|
|oneNoteWebUrl|[externalLink](externallink.md)|Abre o bloco de anotações no OneNote na Web.|

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
