---
title: Tipo de recurso invitationParticipantInfo
description: '**InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.'
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5b8432cf28dd078add91b517f75bc33a71fc4e8134ecff8155c97cc0acc887c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202242"
---
# <a name="invitationparticipantinfo-resource-type"></a>Tipo de recurso invitationParticipantInfo

Namespace: microsoft.graph

Esse recurso é usado para representar a entidade que está sendo convidada para uma chamada de grupo. 

## <a name="properties"></a>Propriedades

| Propriedade                           | Tipo                          | Descrição                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| identity                           | [identitySet](identityset.md) | O [identitySet](identityset.md) associado a esse convite.                   |
| replacesCallId                     | String                        | Opcional. A chamada da qual a identidade de destino faz parte no momento. Essa chamada será retirada depois que o participante for adicionado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "replacesCallId"
  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
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

