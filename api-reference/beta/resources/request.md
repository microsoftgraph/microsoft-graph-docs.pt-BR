---
title: tipo de recurso request
description: Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrono para criar, atualizar e excluir um objeto.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 871f2232e57bdd24aeff9842df699ea0601146eb
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509186"
---
# <a name="request-resource-type"></a>tipo de recurso request

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrono para criar, atualizar e excluir um objeto.

Herda de [entidade](entity.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|String|O identificador da aprovação da solicitação.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação.|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação.|
|createdDateTime|DateTimeOffset|A data de criação da solicitação.|
|customData|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado.|
|status|String|O status da solicitação. Não anulável. Os valores possíveis são: `Canceled`, `Denied`, , `Failed`, `Granted`, `PendingAdminDecision`, `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`, , `Revoked`e `ScheduleCreated`. Não anulável.|
|id|Cadeia de caracteres|Identificador da solicitação. Somente leitura. Não anulável. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aprovação|[aprovação](../resources/approval.md)|Representa o objeto de aprovação ao que a solicitação está vinculada.|

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
  "approvalId": "String (identifier)",
  "completedDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "customData": "String",
  "status": "String",
}
```

