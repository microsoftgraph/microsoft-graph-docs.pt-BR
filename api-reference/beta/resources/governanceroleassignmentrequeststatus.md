---
title: Tipo de recurso governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 19eb182a450053400b66db12c0d2fe119908a992
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510201"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>Tipo de recurso governanceRoleAssignmentRequestStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                                            | Descrição                                                                                                                                                                                                                                                                                                                                                                                     |
| :------------ | :---------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| status        | Cadeia de caracteres                                          | O status da solicitação de atribuição de função. O valor pode ser `InProgress` ou `Closed`.                                                                                                                                                                                                                                                                                                           |
| subStatus     | Cadeia de caracteres                                          | O sub status da solicitação de atribuição de função. Os valores podem ser `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, , `PendingProvisioning`, `Provisioned`, `PendingRevocation`, , `Canceled``Revoked`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, , `PendingAdminDecision`, `AdminApproved``AdminDenied`, , `TimedOut`e `ProvisioningStarted`. |
| statusDetails | Coleção [KeyValue](../resources/keyvalue.md) | Os detalhes do status da solicitação de atribuição de função. Representa os resultados de avaliação de regras diferentes.                                                                                                                                                                                                                                                                              |

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
