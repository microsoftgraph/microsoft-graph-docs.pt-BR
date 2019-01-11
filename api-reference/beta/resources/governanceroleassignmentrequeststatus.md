---
title: tipo de recurso de governanceRoleAssignmentRequestStatus
description: Representa o status do governanceRoleAssignmentRequest.
localization_priority: Normal
ms.openlocfilehash: c5daac53661cc607d51e5bfd1ec9031cfa599fca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808068"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a>tipo de recurso de governanceRoleAssignmentRequestStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o status do [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).


## <a name="properties"></a>Propriedades
Propriedade       | Tipo |Descrição|
|:----|:-------------|:-----|
|status |Cadeia de caracteres| O status da solicitação de atribuição de função. O valor pode ser `InProgress` ou `Closed`.|
|subStatus |Cadeia de caracteres| O status de sub da solicitação de atribuição de função. Os valores podem ser `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, e `ProvisioningStarted`.|
|statusDetails       |coleção [keyValue](../resources/keyvalue.md)| Os detalhes do status da solicitação de atribuição de função. Ele representa os resultados de avaliação de regras diferentes. |

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
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
