---
title: Tipo de recurso unifiedApprovalStage
description: Define as configurações dos estágios de aprovação em um objeto unifiedRoleManagementPolicyApprovalRule.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b046071cb3468187d75ebd079b4329907e3550c5
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133927"
---
# <a name="unifiedapprovalstage-resource-type"></a>Tipo de recurso unifiedApprovalStage

Namespace: microsoft.graph

Define as configurações dos estágios de aprovação em um [objeto unifiedRoleManagementPolicyApprovalRule](unifiedrolemanagementpolicyapprovalrule.md) . Especifica os aprovadores primário e escalonamento de cada estágio e se aprovações e escalonamentos são necessários.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalStageTimeOutInDays|Int32| O número de dias que uma solicitação pode estar aguardando uma resposta antes que ela seja negada automaticamente. |
|escalationApprovers|[coleção subjectSet](../resources/subjectset.md)| Os aprovadores de escalonamento para esse estágio quando os aprovadores primários não respondem.|
|escalationTimeInMinutes|Int32|O tempo em que uma solicitação pode estar pendente de uma resposta de um aprovador primário antes que ela possa ser escalonada para os aprovadores de escalonamento.|
|isApproverJustificationRequired|Booliano| Indica se o aprovador deve fornecer justificativa para sua resposta.|
|isEscalationEnabled|Booliano| Indica se o escalonamento está habilitado.|
|primaryApprovers|[coleção subjectSet](../resources/subjectset.md)| Os principais aprovadores deste estágio.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unifiedApprovalStage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedApprovalStage",
  "approvalStageTimeOutInDays": "Integer",
  "isApproverJustificationRequired": "Boolean",
  "escalationTimeInMinutes": "Integer",
  "primaryApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "isEscalationEnabled": "Boolean",
  "escalationApprovers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ]
}
```

