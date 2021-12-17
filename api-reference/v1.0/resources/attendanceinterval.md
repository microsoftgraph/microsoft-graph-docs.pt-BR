---
title: tipo de recurso attendanceInterval
description: Contém informações associadas a um intervalo de participação em um attendanceRecord.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 643dcfa2e7c032fba93af164271150c41b6693b2
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547502"
---
# <a name="attendanceinterval-resource-type"></a>tipo de recurso attendanceInterval

Namespace: microsoft.graph

Contém informações associadas a um intervalo de presença em [um attendanceRecord](attendancerecord.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| durationInSeconds | Int32 | Duração do intervalo de reunião em segundos; ou seja, a diferença entre **joinDateTime** e **leaveDateTime**. |
| joinDateTime | DateTime | A hora em que o participante ingressou no UTC. |
| leaveDateTime | DateTime | A hora em que o participante foi embora em UTC. |

> [!TIP]
> Quando os dados não estão disponíveis, o valor de **joinDateTime** ou **leaveDateTime** será definido como , e o valor de durationInSeconds será definido como no corpo da resposta do `null` método Get  `0` [meetingAttendanceReport.](/graph/api/meetingattendancereport-get?view=graph-rest-v1.0&preserve-view=true)

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
