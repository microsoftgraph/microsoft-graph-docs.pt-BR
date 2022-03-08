---
title: tipo complexo approvalStage
description: Usada para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote de acesso. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd5a27a66d335dfe56acfbb0d30771ddbd9a703c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336379"
---
# <a name="approvalstage-complex-type"></a>tipo complexo approvalStage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usada para a **propriedade approvalStages** das configurações de aprovação **na propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso](accesspackageassignmentpolicy.md). Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | O número de dias em que uma solicitação pode estar pendente de uma resposta antes de ser negada automaticamente. |
| isApproverJustificationRequired |Booliano | Indica se o aprovador é necessário para fornecer uma justificativa para aprovar uma solicitação. |
| isEscalationEnabled |Booliano | Se for true, um ou mais aprovadores de escalonamento serão configurados neste estágio de aprovação. |
| escalationTimeInMinutes |Int32 | Se a escalação for necessária, o tempo em que uma solicitação poderá estar pendente de uma resposta de um aprovador primário. |
| primaryApprovers | [Coleção userSet](userset.md)| Os usuários que serão solicitados a aprovar solicitações. Uma coleção [de singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md). Ao criar ou atualizar uma [política](accesspackageassignmentpolicy.md), inclua pelo menos um **userSet** nesta coleção. |
| escalationApprovers | [Coleção userSet](userset.md)| Se a escalonamento estiver habilitada e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers serão os usuários que serão solicitados a aprovar solicitações. Pode ser uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).  Ao criar ou atualizar uma [política, se](accesspackageassignmentpolicy.md) não houver aprovadores de escalonamento ou aprovadores de escalonamento não são necessários para o estágio, o valor dessa propriedade deve ser uma coleção vazia.|



## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do estágio de aprovação de solicitação.

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


