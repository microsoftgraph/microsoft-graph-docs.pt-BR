---
title: Tipo de recurso meetingAttendanceReport
description: Contém informações associadas a um relatório de participação na reunião.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 46b996cf9eb1212fdbd4cc6ee968df719a5264e3
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547497"
---
# <a name="meetingattendancereport-resource-type"></a>Tipo de recurso meetingAttendanceReport

Namespace: microsoft.graph

Contém informações associadas a um relatório de participação na reunião.

Os relatórios de participação da reunião são artefatos de reunião online. Para obter detalhes, consulte [Artefatos e permissões de](/graph/cloud-communications-online-meeting-artifacts)reunião online.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar meetingAttendanceReports](../api/meetingattendancereport-list.md)|[coleção meetingAttendanceReport](../resources/meetingattendancereport.md)|Obter uma lista de  [objetos meetingAttendanceReport](../resources/meetingattendancereport.md) e suas propriedades.|
|[Obter meetingAttendanceReport](../api/meetingattendancereport-get.md)|[meetingAttendanceReport](../resources/meetingattendancereport.md)|Leia as propriedades e as relações de um [objeto meetingAttendanceReport.](../resources/meetingattendancereport.md)|

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                               | Descrição                     |
|:----------------------|:---------------------------------------------------|:--------------------------------|
| id                    | Cadeia de caracteres   | Identificador exclusivo do relatório de presença. Somente leitura. |
| meetingEndDateTime    | DateTimeOffset | Hora UTC quando a reunião terminou. Somente leitura.   |
| meetingStartDateTime  | DateTimeOffset | Hora UTC quando a reunião começou. Somente leitura.   |
| totalParticipantCount | Int32 | Número total de participantes. Somente leitura.  |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
| ------------ | ---- | ----------- |
| attendanceRecords | [coleção attendanceRecord](attendanceRecord.md) | Lista de registros de presença de um relatório de participação. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```json
{
  "@odata.type": "#microsoft.graph.meetingAttendanceReport",
  "id": "String(identifier)",
  "meetingEndDateTime": "String (timestamp)",
  "meetingStartDateTime": "String (timestamp)",
  "totalParticipantCount": "Int32",

  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
