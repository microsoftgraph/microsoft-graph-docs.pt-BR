---
title: tipo de recurso attendanceInterval
description: Contém informações associadas ao intervalo de participação no attendanceRecord.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13b4e20a5233b865dd5417eed4d159bce07c8717
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896512"
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
