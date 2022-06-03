---
title: Tipo de recurso meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d46f15a86742a23b6ec4e9f6c270308de34c169c
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883982"
---
# <a name="meetingparticipantinfo-resource-type"></a>Tipo de recurso meetingParticipantInfo

Namespace: microsoft.graph

Informações sobre um participante em uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo                          | Descrição                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| Identidade | [identitySet](identityset.md) | Informações de identidade do participante.                                            |
| Upn      | String                        | Nome principal do usuário do participante.                                             |
| role     | onlineMeetingRole             | Especifica a função do participante na reunião.  Os valores possíveis `attendee`são `presenter`, `producer`e `unknownFutureValue`.|

> [!TIP]
>
> Para definir a  **função de apresentador** de um participante da reunião ao criar ou atualizar um [onlineMeeting](onlinemeeting.md), o valor de **allowedPresenters** também deve ser definido como `roleIsPresenter`.

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

