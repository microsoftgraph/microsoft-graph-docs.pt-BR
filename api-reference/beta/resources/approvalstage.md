---
title: tipo complexo approvalStage
description: No gerenciamento de direitos, usado para a propriedade approvalStages das configurações de aprovação na propriedade requestApprovalSettings de uma política de atribuição de pacote de acesso. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio. No PIM, define as configurações dos estágios de aprovação em um objeto unifiedRoleManagementPolicyApprovalRule.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cfaf9c314002e5fcc0dd2865216ea4346272e4b3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900055"
---
# <a name="approvalstage-complex-type"></a>tipo complexo approvalStage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos, usado para a propriedade **approvalStages** das configurações de aprovação na propriedade **requestApprovalSettings** de uma política de atribuição [de pacote de acesso](accesspackageassignmentpolicy.md). Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.

No PIM, define as configurações dos estágios de aprovação em um objeto [unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md) . Especifica os aprovadores primário e escalonamento de cada estágio e se aprovações e escalonamentos são necessários.

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| approvalStageTimeOutInDays |Int32 | O número de dias que uma solicitação pode estar aguardando uma resposta antes que ela seja negada automaticamente. |
| isApproverJustificationRequired |Booliano | Indica se o aprovador é necessário para fornecer uma justificativa para aprovar uma solicitação. |
| isEscalationEnabled |Booliano | Se for true, um ou mais aprovadores de escalonamento serão configurados neste estágio de aprovação. |
| escalationTimeInMinutes |Int32 | Se o escalonamento for necessário, o tempo em que uma solicitação poderá estar pendente de uma resposta de um aprovador primário. |
| primaryApprovers | [coleção userSet](userset.md)| Os usuários que serão solicitados a aprovar solicitações. Uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md). Ao criar ou atualizar uma [política](accesspackageassignmentpolicy.md), inclua pelo menos um **userSet** nesta coleção. |
| escalationApprovers | [coleção userSet](userset.md)| Se o escalonamento estiver habilitado e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers serão os usuários que serão solicitados a aprovar solicitações. Pode ser uma coleção de [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) e [externalSponsors](externalsponsors.md).  Ao criar ou atualizar uma [política, se](accesspackageassignmentpolicy.md) não houver aprovadores de escalonamento ou aprovadores de escalonamento não forem necessários para o estágio, o valor dessa propriedade deverá ser uma coleção vazia.|



## <a name="json-representation"></a>Representação JSON

A seguir está uma representação JSON do estágio de aprovação da solicitação.

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


