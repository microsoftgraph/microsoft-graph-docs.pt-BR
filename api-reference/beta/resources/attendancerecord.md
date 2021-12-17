---
title: tipo de recurso attendanceRecord
description: Contém informações associadas a um registro de participação em uma meetingAttendanceReport.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f6f045062f088dcb264cb6485bdd8df6e222e400
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547665"
---
# <a name="attendancerecord-resource-type"></a>tipo de recurso attendanceRecord

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações associadas a um registro de participação em [uma meetingAttendanceReport](meetingattendancereport.md).

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar attendanceRecords](../api/attendancerecord-list.md)|[coleção attendanceRecord](../resources/attendancerecord.md)|Obter uma lista de [objetos attendanceRecord](../resources/attendancerecord.md) e suas propriedades.|

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição|
|:--------------------|:--------|:-----------|
| attendanceIntervals | [coleção attendanceInterval](attendanceinterval.md) | Lista de períodos entre ingressar e sair de uma reunião. |
| emailAddress | String | Endereço de email do usuário associado a esse registro de atenuação. |
| identity | [identity](identity.md) | Identidade do usuário associado a esse registro de atenuação. |
| role | Cadeia de caracteres | Função do participante. Os valores possíveis são: `None`, `Attendee`, `Presenter`, e `Organizer`.  |
| totalAttendanceInSeconds | Int32 | Duração total dos atendimentos em segundos. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attendanceRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.attendanceRecord",
  "emailAddress": "String",
  "totalAttendanceInSeconds": "Int32",
  "role": "String(None|Attendee|Presenter|Organizer)",
  "identity": {
    "@odata.type": "#microsoft.graph.identity"
  },
  "attendanceIntervals": [
    {
      "@odata.type": "#microsoft.graph.attendanceInterval"
    }
  ]
}
```
