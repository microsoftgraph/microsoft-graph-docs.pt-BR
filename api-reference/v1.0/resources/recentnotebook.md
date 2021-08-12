---
title: tipo de recurso recentNotebook
description: Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um notebook, mas tem menos propriedades.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 40a9b71dbf32aebb169b621c9defacc75c0209be8f22afb7f2063675ac0d913d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135026"
---
# <a name="recentnotebook-resource-type"></a>tipo de recurso recentNotebook

Namespace: microsoft.graph

Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome do bloco de anotações.|
|lastAccessedTime|DateTimeOffset|A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|links|[recentNotebookLinks](recentnotebooklinks.md)|Links para abrir o bloco de anotações. O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado. O `oneNoteWebURL` link abre o bloco de anotações OneNote na Web.|
|sourceService|onenoteSourceService|A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | Coleção [Notebook](notebook.md) | Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário. |

