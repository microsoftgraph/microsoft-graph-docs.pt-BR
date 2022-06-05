---
title: tipo de recurso de solicitação
description: Representa os detalhes de uma solicitação no PIM ou userConsentRequests.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 72a52ce4911dc85a5d4f954cdc48e62ad8f1f9c2
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65897949"
---
# <a name="request-resource-type"></a>tipo de recurso de solicitação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma solicitação no [PIM ou](privilegedidentitymanagementv3-overview.md) apIs [de solicitação de consentimento do](userconsentrequest.md) usuário.

Herda de [entidade](../resources/entity.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|String| O identificador da aprovação da solicitação.  |
|completedDateTime|DateTimeOffset| A data de conclusão da solicitação. |
|createdBy|[identitySet](../resources/identityset.md)|A entidade de segurança que criou a solicitação.|
|createdDateTime|DateTimeOffset|A data de criação da solicitação.|
|Customdata|Cadeia de Caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado.|
|id|String|O identificador exclusivo do objeto de solicitação. Herdado da [entidade](../resources/entity.md).|
|status|String| O status da solicitação. Não anulável. Os valores possíveis são: `Canceled`, `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, , `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`, , `Revoked`e `ScheduleCreated`. Não anulável. |

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