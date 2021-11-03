---
title: Tipo de recurso approvalStep
description: O objeto approvalStep associado a um accessPackageAssignmentRequest ou userConsentRequest.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c1a3b77bb9d6ac48281c0e58c448b1182c6c1930
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730379"
---
# <a name="approvalstep-resource-type"></a>Tipo de recurso approvalStep

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto approvalStep para decisões associadas ao `accessPackageAssignmentRequest` . Ele é usado para distinguir decisões para diferentes etapas de um fluxo de trabalho de aprovação em que os aprovadores podem agir.

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
|displayName|Cadeia de caracteres|O rótulo fornecido pelo criador da política para identificar uma etapa de aprovação. Somente leitura.|
|id|Cadeia de caracteres|O identificador da etapa associada a um objeto de aprovação. Somente leitura.|
|justification|Cadeia de caracteres|A justificativa associada à decisão da etapa de aprovação.|
|reviewResult|Cadeia de caracteres|O resultado desse registro de aprovação. Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .|
|reviewedBy|[Coleção userIdentity](useridentity.md) | O identificador do revistor. Somente leitura.|
|reviewedDateTime|DateTimeOffset|A data e a hora em que uma decisão foi registrada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|status|Cadeia de caracteres|O status da etapa. Valores possíveis: `InProgress` `Initializing` , , , `Completed` `Expired` . Somente leitura.|


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
