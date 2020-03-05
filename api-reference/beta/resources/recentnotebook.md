---
title: tipo de recurso recentNotebook
description: Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um notebook, mas tem menos propriedades.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6a5df3f75a1cf41fa15d59ac987f8f16bb9fdfce
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521261"
---
# <a name="recentnotebook-resource-type"></a>tipo de recurso recentNotebook

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|O nome do bloco de anotações.|
|lastAccessedTime|DateTimeOffset|A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|links|[recentNotebookLinks](recentnotebooklinks.md)|Links para abrir o bloco de anotações. O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado. O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.|
|sourceService|String|A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.|

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
