---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a642532579d127fdeb48b4c69524975b293ff959
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741996"
---
# <a name="meetingparticipantinfo-resource-type"></a>tipo de recurso meetingParticipantInfo

Namespace: microsoft.graph

Informações sobre um participante de uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| ladrões | [identitySet](identityset.md) | Informações de identidade do participante.                                            |
| UPN      | String                        | Nome principal do usuário do participante.                                             |
| role     | onlineMeetingRole             | Especifica a função do participante na reunião.  Os valores possíveis estão listados na tabela a seguir. |

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

