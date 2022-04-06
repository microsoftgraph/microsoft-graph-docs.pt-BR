---
title: Tipo de recurso accessPackageApprovalStage
description: Usada para a propriedade stages das configurações de aprovação. Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cffd48048af6d9b44ef475cdc3adcc6d9f0da05f
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608262"
---
# <a name="accesspackageapprovalstage-complex-type"></a>tipo complexo accessPackageApprovalStage

Namespace: microsoft.graph

Usada para a **propriedade stages** de [configurações de aprovação](accesspackageassignmentapprovalsettings.md) em uma política de atribuição [de pacote de acesso](accesspackageassignmentpolicy.md). Especifica os aprovadores primários, de fallback e de escalonamento de cada estágio.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|durationBeforeAutomaticDenial|Duration|O número de dias em que uma solicitação pode estar pendente de uma resposta antes de ser negada automaticamente.|
|durationBeforeEscalation|Duration|Se a escalação for necessária, o tempo em que uma solicitação poderá estar pendente de uma resposta de um aprovador primário.|
|escalationApprovers|[coleção subjectSet](../resources/subjectset.md)|Se a escalonamento estiver habilitada e os aprovadores primários não responderem antes do tempo de escalonamento, os escalationApprovers serão os usuários que serão solicitados a aprovar solicitações. |
|fallbackEscalationApprovers|[coleção subjectSet](../resources/subjectset.md)|Os assuntos, normalmente usuários, que são os aprovadores de escalonamento de fallback.|
|fallbackPrimaryApprovers|[coleção subjectSet](../resources/subjectset.md)|Os assuntos, normalmente usuários, que são os aprovadores primários de fallback.|
|isApproverJustificationRequired|Boolean|Indica se o aprovador é necessário para fornecer uma justificativa para aprovar uma solicitação.|
|isEscalationEnabled|Booliano|If `true`, then one or **more escalationApprovers** are configured in this approval stage.|
|primaryApprovers|[coleção subjectSet](../resources/subjectset.md)|Os assuntos, normalmente usuários, que serão solicitados a aprovar solicitações. Uma coleção [de singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) ou [externalSponsors](externalsponsors.md).|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageApprovalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageApprovalStage",
  "durationBeforeAutomaticDenial": "String (duration)",
  "isApproverJustificationRequired": "Boolean",
  "isEscalationEnabled": "Boolean",
  "durationBeforeEscalation": "String (duration)",
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackPrimaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackEscalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```


