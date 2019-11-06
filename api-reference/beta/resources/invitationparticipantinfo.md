---
title: tipo de recurso invitationParticipantInfo
description: O **InvitationParticipant** é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 7e25e65fb87f664788b0649f188def29b62c13d2
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006688"
---
# <a name="invitationparticipantinfo-resource-type"></a>tipo de recurso invitationParticipantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Este recurso é usado para representar um conjunto de identidades associadas a um convite de conversa e fornece parâmetros de convite adicionais.

## <a name="properties"></a>Propriedades

| Propriedade                           | Tipo                          | Descrição                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| EndpointType                       | String                        | O tipo de ponto de extremidade. Os valores possíveis são: `default` e `voicemail`. |
| ladrões                           | [identitySet](identityset.md) | O [identityset](identityset.md) associado a este convite.                   |
| languageId                         | String                        | A cadeia de caracteres de cultura do idioma.                                                                                     |
| região                             | String                        | Região do participante.                                                           |
| replacesCallId                     | String                        | Opcional. A chamada na qual o idenity de destino faz parte no momento. Essa chamada será cancelada quando o participante for adicionado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
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
