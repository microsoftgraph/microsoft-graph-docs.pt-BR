---
title: Tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: e04b49fedf761ef3715d152fdc2a07a3af139bc3
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695409"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Tipo de recurso governanceRoleAssignmentRequestStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Propriedades
Propriedade       | Tipo |Descrição|
|:----|:-------------|:-----|
|status |String| O status da solicitação de atribuição de função. O valor pode ser `InProgress` ou `Closed` .|
|subStatus |String| O sub status da solicitação de atribuição de função. Os valores podem `Accepted` ser , , , , , , , , `PendingEvaluation` , , , `Granted` , , `Denied` , , , , `PendingProvisioning` , `Provisioned` `PendingRevocation` e `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` .|
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


