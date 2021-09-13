---
title: Tipo de recurso usageDetails
description: Tipo complexo que contém propriedades de itens usados. Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3924577830b67733fd2e967fa9de4a30b1473492
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118534"
---
# <a name="usagedetails-resource-type"></a>Tipo de recurso usageDetails

Namespace: microsoft.graph

Tipo complexo que contém propriedades de [itens usados.](insights-used.md) Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo          | Descrição  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | A data e a hora em que o recurso foi acessado pela última vez pelo usuário. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.                     |
| lastModifiedDateTime              | DateTimeOffset        | A data e a hora em que o recurso foi modificado pela última vez pelo usuário. O data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` . Somente leitura.       |

