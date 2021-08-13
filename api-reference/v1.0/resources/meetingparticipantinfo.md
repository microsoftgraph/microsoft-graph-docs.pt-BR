---
title: Tipo de recurso meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f262c6b2b13dc430173e585f6afa25c231bfea858b52bc56803a726ba893acff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126400"
---
# <a name="meetingparticipantinfo-resource-type"></a>Tipo de recurso meetingParticipantInfo

Namespace: microsoft.graph

Informações sobre um participante em uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| identity | [identitySet](identityset.md) | Informações de identidade do participante.                                            |
| upn      | Cadeia de caracteres                        | Nome principal do usuário do participante.                                             |
| role     | onlineMeetingRole             | Especifica a função do participante na reunião.  Os valores possíveis são: `attendee`, `presenter` e `unknownFutureValue`.|

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

