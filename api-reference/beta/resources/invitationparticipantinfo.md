---
title: Tipo de recurso invitationParticipantInfo
description: Representa uma entidade que está sendo convidada para uma chamada de grupo.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 16885239d0af9be8e9e8e66eade8f75c2d120a8e
ms.sourcegitcommit: 089669703041900c4700c5d4f383ed05a7f193f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/04/2022
ms.locfileid: "65191637"
---
# <a name="invitationparticipantinfo-resource-type"></a>Tipo de recurso invitationParticipantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entidade que está sendo convidada para uma chamada de grupo. 

## <a name="properties"></a>Propriedades

| Propriedade                           | Tipo                          | Descrição                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| Endpointtype                       | Cadeia de Caracteres                        | O tipo do ponto de extremidade. Os valores possíveis são: `default` e `voicemail`. |
| identity                           | [identitySet](identityset.md) | O [identitySet](identityset.md) associado a este convite.                   |
| participantId                      | String                        | Opcional. A ID do participante de destino.                                          |
| replacesCallId                     | String                        | Opcional. A chamada da qual a identidade de destino faz parte no momento. Para casos ponto a ponto, a chamada será descartada depois que o participante for adicionado com êxito. |

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
  "endpointType": "String",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "participantId": "String",  
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


