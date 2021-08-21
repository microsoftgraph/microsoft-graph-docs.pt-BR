---
title: tipo de recurso request
description: Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrono para criar, atualizar e excluir um objeto.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 66856dada00835db637b86c8d1577ea83740c7e1
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454273"
---
# <a name="request-resource-type"></a>tipo de recurso request

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrono para criar, atualizar e excluir um objeto.

Herda da [entidade](entity.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|Cadeia de caracteres|O identificador da aprovação da solicitação.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação.|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação.|
|createdDateTime|DateTimeOffset|A data de criação da solicitação.|
|customData|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado.|
|status|Cadeia de caracteres|O status da solicitação. Não anulável. Os valores possíveis são: `Canceled` , , , , , , , , , `Denied` , , e `Failed` `Granted` `PendingAdminDecision` `PendingApproval` `PendingProvisioning` `PendingScheduleCreation` `Provisioned` `Revoked` `ScheduleCreated` . Não anulável.|
|id|Cadeia de caracteres|Identificador da solicitação. Somente leitura. Não anulável. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relacionamentos
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

