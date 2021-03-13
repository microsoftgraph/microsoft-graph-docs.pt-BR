---
title: Tipo de recurso approvalStep
description: O objeto approvalStep associado ao accessPackageAssignmentRequest.
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 263e809e5858cdc23b34b8401171bb5fce668721
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761251"
---
# <a name="approvalstep-resource-type"></a>Tipo de recurso approvalStep

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), o objeto approvalStep para decisões associadas ao `accessPackageAssignmentRequest` . Ele é usado para distinguir decisões para diferentes etapas de um fluxo de trabalho de aprovação em que os aprovadores podem agir.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
|[Aprovação de listaSteps](../api/approval-list-steps.md) | [Coleção approvalStep](approvalstep.md) | Listar **os objetos approvalStep** associados a um **objeto de** aprovação. |
|[Obter approvalStep](../api/approvalstep-get.md) | [approvalStep](approvalstep.md) | Recupere as propriedades de um **objeto approvalStep.** |
|[Atualizar approvalStep](../api/approvalstep-update.md) | Nenhum | Aplicar aprovar ou negar decisão em um **objeto approvalStep.** |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador da etapa associada a um objeto de aprovação. Somente leitura.|
|displayName|Cadeia de caracteres|O rótulo fornecido pelo criador da política para identificar uma etapa de aprovação. Somente leitura|
|status|Cadeia de caracteres|O status da etapa. Valores possíveis: `InProgress` ou `Completed` . Somente leitura.|
|assignedToMe|Boolean|Indica se a etapa é atribuída ao usuário chamador para revisar. Somente leitura.|
|reviewedBy|[Coleção userIdentity](useridentity.md) | O identificador do revistor. Somente leitura.|
|reviewedDateTime|DateTimeOffset|A data e a hora em que uma decisão foi registrada. Somente leitura.|
|reviewResult|Cadeia de Caracteres|O resultado desse registro de aprovação. Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .|
|justification|Cadeia de Caracteres|A justificativa associada à decisão da etapa de aprovação.|

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
  "@odata.type": "#microsoft.graph.approvalStep",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": true,
  "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String",
}
```
