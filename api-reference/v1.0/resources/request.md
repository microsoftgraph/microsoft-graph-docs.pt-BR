---
title: tipo de recurso de solicitação
description: Representa os detalhes de uma solicitação no PIM ou userConsentRequests
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e8702ef1b0bc091e5d2e24e2808a86cefbd82b9f
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133864"
---
# <a name="request-resource-type"></a>tipo de recurso de solicitação

Namespace: microsoft.graph

Representa os detalhes de uma solicitação no [PIM ou](privilegedidentitymanagementv3-overview.md) apIs [de solicitação de consentimento do](userconsentrequest.md) usuário.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

Nenhum.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|Cadeia de caracteres| O identificador da aprovação da solicitação.  |
|completedDateTime|DateTimeOffset| A data de conclusão da solicitação. |
|createdBy|[identitySet](../resources/identityset.md)|A entidade de segurança que criou a solicitação.|
|createdDateTime|DateTimeOffset|A data de criação da solicitação.|
|Customdata|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado.|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de solicitação. Herdado da [entidade](../resources/entity.md).|
|status|Cadeia de caracteres| O status da solicitação. Não anulável. Os valores possíveis são: `Canceled`, `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, , `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`, , `Revoked`e `ScheduleCreated`. Não anulável. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.request",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.request",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

