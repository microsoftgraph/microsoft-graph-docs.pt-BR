---
title: tipo complexo approvalStage
description: Usado para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote do Access. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 158fae1675c26876daeb05b1571d7fd91855df72
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777698"
---
# <a name="approvalstage-complex-type"></a>tipo complexo approvalStage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a propriedade **approvalStages** das configurações de aprovação na propriedade **requestApprovalSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | O número de dias que uma solicitação pode aguardar uma resposta antes de ser automaticamente negada. |
| isApproverJustificationRequired |Booliano | Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação. |
| isEscalationEnabled |Booliano | Se true, um ou mais aprovadores de escalonamento estão configurados neste estágio de aprovação. |
| escalationTimeInMinutes |Int32 | Se for necessário escalonamento, o tempo em que uma solicitação pode ser pendente é uma resposta de um Aprovador principal. |
| primaryApprovers | coleção [userset](userset.md)| Os usuários que serão solicitados a aprovar solicitações. Uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md). |
| escalationApprovers | coleção [userset](userset.md)| Se o escalonamento estiver habilitado e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers são os usuários que serão solicitados a aprovar solicitações. Pode ser uma coleção de [únicousuário](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).|



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON da fase solicitar aprovação.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage"
}-->

```json

{
    "approvalStageTimeOutInDays": 14,
    "isApproverJustificationRequired": true,
    "isEscalationEnabled": true,
    "escalationTimeInMinutes": 11520,
    "primaryApprovers": [{"@odata.type": "microsoft.graph.userSet"}],
    "escalationApprovers": [{"@odata.type": "microsoft.graph.userSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


