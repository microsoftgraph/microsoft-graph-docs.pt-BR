---
title: Tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 80994db594c2f0e45dfe36a5fbf32260266a0536
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453538"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Tipo de recurso governanceRoleAssignmentRequestStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Propriedades
Propriedade       | Tipo |Descrição|
|:----|:-------------|:-----|
|status |Cadeia de caracteres| O status da solicitação de atribuição de função. O valor pode ser `InProgress` ou `Closed` .|
|subStatus |Cadeia de caracteres| O sub status da solicitação de atribuição de função. Os valores podem `Accepted` ser , , , , , , , , `PendingEvaluation` , , , `Granted` , , `Denied` , , , , `PendingProvisioning` , `Provisioned` `PendingRevocation` e `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` .|
|statusDetails       |Coleção [KeyValue](../resources/keyvalue.md)| Os detalhes do status da solicitação de atribuição de função. Representa os resultados de avaliação de regras diferentes. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


