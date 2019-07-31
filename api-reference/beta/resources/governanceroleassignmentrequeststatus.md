---
title: tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ca61e5e3ef5456889eafcef3914f16fc072dfb6b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971854"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>tipo de recurso governanceRoleAssignmentRequestStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Propriedades
Propriedade       | Tipo |Descrição|
|:----|:-------------|:-----|
|status |String| O status da solicitação de atribuição de função. O valor pode ser `InProgress` ou `Closed`.|
|substatus |String| O status da solicitação de atribuição de função. Os valores podem ser `Accepted`, `PendingEvaluation` `Granted` `Denied` `PendingProvisioning` `Provisioned` `AdminApproved` `AdminDenied` `PendingAdminDecision` `PendingApproval` `Failed` `PendingApprovalProvisioning` `FailedAsResourceIsLocked` `TimedOut`,,,,,,,,,,,,,, e `ProvisioningStarted` `PendingRevocation` `Revoked` `Canceled`|
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
