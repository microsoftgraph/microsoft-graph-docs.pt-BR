---
title: Tipo de recurso meetingParticipantInfo
description: Informações sobre um participante em uma reunião.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5d3f8e5fb055fa45ef150aa9ef7eef82980d0755
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2022
ms.locfileid: "63668581"
---
# <a name="meetingparticipantinfo-resource-type"></a>Tipo de recurso meetingParticipantInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre um participante em uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo             | Descrição                 |
| :------- | :-------------------- | :------------------------------ |
| identity | [identitySet](identityset.md) | Informações de identidade do participante.           |
| upn      | String                        | Nome principal do usuário do participante.             |
| role     | [onlineMeetingRole](#onlinemeetingrole-values)     | Especifica a função do participante na reunião.|

### <a name="onlinemeetingrole-values"></a>Valores onlineMeetingRole

A tabela a seguir lista os membros de [uma enumeração evolvável](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations). Você deve usar o `Prefer: include-unknown-enum-members` header de solicitação para obter o `coorganizer` valor neste número evolvável.

| Valor              | Descrição                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| attendee            | A função do participante é participante. Esse valor se aplica a todas as reuniões.   |
| apresentador           | A função do participante é apresentador. Esse valor se aplica a reuniões com **allowedPresenter** definido como `roleIsPresenter`, ou um evento Teams ao vivo. |
| producer            | A função do participante é produtor. Esse valor se aplica somente Teams evento ao vivo.  |
| coorganizador | A função do participante é co-organizadora. Esse valor se aplica a todas as reuniões, exceto Teams evento ao vivo. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |

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


