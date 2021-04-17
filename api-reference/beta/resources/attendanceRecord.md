---
title: tipo de recurso attendanceRecord
description: Contém informações associadas ao registro de participação no relatório de participação da reunião.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 025c878d8778604bab34dda15f6ab0fa2c541151
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882632"
---
# <a name="attendancerecord-resource-type"></a>tipo de recurso attendanceRecord

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações associadas ao registro de participação no relatório de participação da reunião.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| identity | [Identidade](identity.md) | Identificador, como nome para exibição. |
| emailAddress | String | Endereço de email. |
| totalAttendanceInSeconds | Int32 | Duração total dos atendimentos em segundos. |
| attendanceIntervals | [coleção attendanceInterval](attendanceInterval.md) | Lista de períodos entre a junção e a saída. |
| role | Cadeia de caracteres | Função do participante. Os valores possíveis `None` `Attendee` são , e `Presenter` `Organizer` .  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceRecord"
}-->

```json

{
    "emailAddress": "String",
    "totalAttendanceInSeconds": "Int32",
    "role": "String(None|Attendee|Presenter|Organizer)",
    "identity": {"@odata.type": "#microsoft.graph.identity"},
    "attendanceIntervals": [{"@odata.type": "#microsoft.graph.attendanceInterval"}]
}

```
