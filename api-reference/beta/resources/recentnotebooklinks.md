---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 5ccf861541526a1673d6174176cb8b2a62df6c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812870"
---
# <a name="recentnotebooklinks-resource-type"></a>tipo de recurso recentNotebookLinks

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.|
|oneNoteWebUrl|[externalLink](externallink.md)|Abre o bloco de anotações no OneNote Online.|

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
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
