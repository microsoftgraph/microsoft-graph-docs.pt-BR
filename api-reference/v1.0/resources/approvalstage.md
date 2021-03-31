---
title: Tipo de recurso approvalStage
description: O objeto approvalStage associado a um userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d6212553d9364c4352bf1d6796156a4020854bf1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469497"
---
# <a name="approvalstage-resource-type"></a>Tipo de recurso approvalStage

Namespace: microsoft.graph

Especifica estágios de decisão na aprovação.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedToMe|Booliano|Indica se o estágio é atribuído ao usuário chamador para revisar. Somente leitura.|
|displayName|String|O rótulo fornecido pelo criador da política para identificar um estágio de aprovação. Somente leitura.|
|id|String|O identificador do estágio associado a um objeto de aprovação. Somente leitura.|
|justification|String|A justificativa associada à decisão do estágio de aprovação.|
|reviewResult|String|O resultado desse registro de aprovação. Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .|
|reviewedBy|[userIdentity](useridentity.md) | O identificador do revistor. Somente leitura.|
|reviewedDateTime|DateTimeOffset|A data e a hora em que uma decisão foi registrada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|status|String|O status do estágio. Valores possíveis: `InProgress` `Initializing` , , , `Completed` `Expired` . Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```
