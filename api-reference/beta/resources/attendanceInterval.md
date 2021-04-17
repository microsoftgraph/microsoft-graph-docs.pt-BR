---
title: tipo de recurso attendanceInterval
description: Contém informações associadas ao intervalo de participação no attendanceRecord.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1746adc802534f72aa9d139c6a16d8da62dd9fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882642"
---
# <a name="attendanceinterval-resource-type"></a>tipo de recurso attendanceInterval

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações associadas ao intervalo de participação no attendanceRecord.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| joinDateTime | DateTime | Participante do horário ingressado em UTC. |
| leaveDateTime | DateTime | O participante do horário foi deixado em UTC. |
| durationInSeconds | Int32 | Duração do intervalo de reunião em segundos; ou seja, a diferença entre **joinDateTime** e **leaveDateTime**. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceInterval"
}-->

```json

{
    "joinDateTime": "String (timestamp)",
    "leaveDateTime": "String (timestamp)",
    "durationInSeconds": "Int32"
}
    
```
