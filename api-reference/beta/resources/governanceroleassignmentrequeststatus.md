---
title: tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 9b0af5326bb9c819ded03ab9497e155cb0dab7c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081682"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>tipo de recurso governanceRoleAssignmentRequestStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Propriedades
Propriedade       | Tipo |Descrição|
|:----|:-------------|:-----|
|status |String| O status da solicitação de atribuição de função. O valor pode ser `InProgress` ou `Closed` .|
|substatus |Cadeia de caracteres| O status da solicitação de atribuição de função. Os valores podem ser,,,,,,,, `Accepted` `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` `PendingRevocation` `Revoked` `Canceled` `Failed` , `PendingApprovalProvisioning` ,, `PendingApproval` `FailedAsResourceIsLocked` , `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` ,,, e.|
|statusDetails       |Coleção [KeyValue](../resources/keyvalue.md)| Os detalhes do status da solicitação de atribuição de função. Ele representa os resultados de avaliação de regras diferentes. |

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


