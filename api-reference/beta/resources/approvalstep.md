---
title: Tipo de recurso approvalStep
description: O objeto approvalStep associado a um accessPackageAssignmentRequest ou userConsentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 510903f27dd751ac57b7df7dab0084f8ce89e35c
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651362"
---
# <a name="approvalstep-resource-type"></a>Tipo de recurso approvalStep

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), o objeto approvalStep para decisões associadas ao `accessPackageAssignmentRequest` . Ele é usado para distinguir decisões para diferentes etapas de um fluxo de trabalho de aprovação em que os aprovadores podem agir.

Em [userConsentRequests](../resources/userconsentrequest.md), as decisões de aprovação associadas a uma solicitação.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Aprovação de listaSteps](../api/approval-list-steps.md) | [Coleção approvalStep](approvalstep.md) | Listar **os objetos approvalStep** associados a um **objeto de** aprovação. |
|[Obter approvalStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Recupere as propriedades de um **objeto approvalStep.** |
|[Atualizar approvalStep](../api/approvalstep-update.md) | Nenhum | Aplicar aprovar ou negar decisão em um **objeto approvalStep.** |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedToMe|Booliano|Indica se a etapa é atribuída ao usuário chamador para revisar. Somente leitura.|
|displayName|String|O rótulo fornecido pelo criador da política para identificar uma etapa de aprovação. Somente leitura.|
|id|String|O identificador da etapa associada a um objeto de aprovação. Somente leitura.|
|justification|String|A justificativa associada à decisão da etapa de aprovação.|
|reviewResult|String|O resultado desse registro de aprovação. Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .|
|reviewedBy|[Coleção userIdentity](useridentity.md) | O identificador do revistor. Somente leitura.|
|reviewedDateTime|DateTimeOffset|A data e a hora em que uma decisão foi registrada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|status|String|O status da etapa. Valores possíveis: `InProgress` `Initializing` , , , `Completed` `Expired` . Somente leitura.|


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aprovação|[coleção approval](../resources/approval.md)|O objeto de aprovação para decisões associadas ao `accessPackageAssignmentRequest` .|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
   "@odata.type":"#microsoft.graph.approvalStep",
   "id":"String (identifier)",
   "displayName":"String",
   "status":"String",
   "assignedToMe":true,
   "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
   "reviewedDateTime":"String (timestamp)",
   "reviewResult":"String",
   "justification":"String"
}
```
