---
title: Tipo de recurso usageDetails
description: Tipo complexo que contém propriedades de itens usados. Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1fe25cc2bab141b3ac29e47b4bca80d8dc24fbe7be410be32398475c9e9a7d14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216837"
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
| lastAccessedDateTime                  | DateTimeOffset        | A data e a hora em que o recurso foi acessado pela última vez pelo usuário. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.                      |
| lastModifiedDateTime              | DateTimeOffset        | A data e a hora em que o recurso foi modificado pela última vez pelo usuário. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`. Somente leitura.       |

