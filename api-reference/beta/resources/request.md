---
title: tipo de recurso de solicitação
description: Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrona para criar, atualizar e excluir um objeto.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6e75c2d632356fceffaf432fc4def204e837c9bc
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399394"
---
# <a name="request-resource-type"></a>tipo de recurso de solicitação

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo de entidade abstrata para modelar o fluxo de trabalho de solicitação assíncrona para criar, atualizar e excluir um objeto.

Herda de [entidade](entity.md).


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|approvalId|Cadeia de caracteres|O identificador da aprovação da solicitação.|
|completedDateTime|DateTimeOffset|A data de conclusão da solicitação.|
|createdBy|[identitySet](identityset.md)|O usuário que criou essa solicitação.|
|createdDateTime|DateTimeOffset|A data de criação da solicitação.|
|Customdata|Cadeia de caracteres|Campo de texto livre para definir quaisquer dados personalizados para a solicitação. Não usado.|
|status|Cadeia de caracteres|O status da solicitação. Não anulável. Os valores possíveis são: `Canceled`, `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, , `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`, , `Revoked`e `ScheduleCreated`. Não anulável.|
|id|Cadeia de caracteres|Identificador da solicitação. Somente leitura. Não anulável. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|aprovação|[aprovação](../resources/approval.md)|Representa o objeto de aprovação ao qual a solicitação está vinculada.|

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

