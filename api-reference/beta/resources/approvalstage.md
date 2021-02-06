---
title: tipo complexo approvalStage
description: Usada para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma diretiva de atribuição de pacote de acesso. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d24f8def3520cf2605f30dc47ab06f52e09fc163
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135251"
---
# <a name="approvalstage-complex-type"></a>tipo complexo approvalStage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a **propriedade approvalStages** das configurações de aprovação na **propriedade requestApprovalSettings** de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | O número de dias que uma solicitação pode estar aguardando uma resposta antes de ser negada automaticamente. |
| isApproverJustificationRequired |Boolean | Indica se o aprovador deve fornecer uma justificativa para aprovar uma solicitação. |
| isEscalationEnabled |Boolean | Se for verdadeiro, um ou mais aprovadores de escalonamento serão configurados nesse estágio de aprovação. |
| escalationTimeInMinutes |Int32 | Se o escalonamento for necessário, o tempo em que uma solicitação poderá estar aguardando uma resposta de um aprovador primário. |
| primaryApprovers | [Coleção userSet](userset.md)| Os usuários que serão solicitados a aprovar solicitações. Uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md). |
| escalationApprovers | [Coleção userSet](userset.md)| Se o escalonamento estiver habilitado e os aprovadores principais não responderem antes do tempo de escalonamento, os escalationApprovers serão os usuários que serão solicitados a aprovar as solicitações. Pode ser uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).|



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


