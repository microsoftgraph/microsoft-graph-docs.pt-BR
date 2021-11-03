---
title: tipo de recurso request
description: Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrono para criar, atualizar e excluir um objeto.
author: carolinetempleton
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fad1d480fbb792ca63b05ddfe8507b2ede9d54e8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695248"
---
# <a name="request-resource-type"></a>tipo de recurso request

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrono para criar, atualizar e excluir um objeto.

Herda da [entidade](entity.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|String|O identificador da aprovação da solicitação.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação.|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação.|
|createdDateTime|DateTimeOffset|A data de criação da solicitação.|
|customData|String|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado.|
|status|String|O status da solicitação. Não anulável. Os valores possíveis são: `Canceled` , , , , , , , , , `Denied` , , e `Failed` `Granted` `PendingAdminDecision` `PendingApproval` `PendingProvisioning` `PendingScheduleCreation` `Provisioned` `Revoked` `ScheduleCreated` . Não anulável.|
|id|String|Identificador da solicitação. Somente leitura. Não anulável. Herdado da [entidade](entity.md).|

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

