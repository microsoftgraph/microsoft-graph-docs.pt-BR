---
title: tipo de recurso invitationParticipantInfo
description: Representa uma entidade que está sendo convidada para uma chamada de grupo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a21ffce09a7f086bced5416eace2a95170b3eaf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523181"
---
# <a name="invitationparticipantinfo-resource-type"></a>tipo de recurso invitationParticipantInfo

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entidade que está sendo convidada para uma chamada de grupo. 

## <a name="properties"></a>Propriedades

| Propriedade                           | Tipo                          | Descrição                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| EndpointType                       | String                        | O tipo de ponto de extremidade. Os valores possíveis são: `default` e `voicemail`. |
| ladrões                           | [identitySet](identityset.md) | O [identityset](identityset.md) associado a este convite.                   |
| replacesCallId                     | String                        | Opcional. A chamada na qual o idenity de destino faz parte no momento. Essa chamada será cancelada quando o participante for adicionado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "endpointType",
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
