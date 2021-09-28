---
title: tipo de recurso attendanceInterval
description: Contém informações associadas ao intervalo de participação no attendanceRecord.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 55b218cfcecb4f2f7d3d597881b612e36fe42860
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979247"
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

> [!TIP]
> Quando os dados não estão disponíveis, o valor de **joinDateTime** ou **leaveDateTime** será definido como , e o valor de `null` **durationInSeconds** será definido como no corpo da resposta da operação Obter relatório de participação da `0` reunião. [](/graph/api/onlinemeeting-get?view=graph-rest-beta&preserve-view=true)

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
