---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e77322dee3f8d94fe8eaee226dce029133a578d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635191"
---
# <a name="meetingparticipantinfo-resource-type"></a>tipo de recurso meetingParticipantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um participante de uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| ladrões | [identitySet](identityset.md) | Informações de identidade do participante.                                           |
| UPN      | String                        | Nome principal do usuário do participante.                                            |
| role     | onlineMeetingRole             | Especifica a função do participante na reunião.  Os valores possíveis são: `attendee`, `presenter` e `unknownFutureValue`.|

### <a name="onlinemeetingrole-values"></a>valores de onlineMeetingRole

| Valor              | Descrição                     |
| ------------------ | ------------------------------- |
| attendee           | O participante é um participante. |
| instrutor          | O participante é um apresentador. |
| unknownFutureValue | Valor de futuro desconhecido.           |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


