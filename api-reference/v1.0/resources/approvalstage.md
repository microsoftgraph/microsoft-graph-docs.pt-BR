---
title: Tipo de recurso approvalStage
description: O objeto approvalStage associado a um userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 49629542b36d7724b17406c14d925844873c8c964334c71b5eec81451376783c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147109"
---
# <a name="approvalstage-resource-type"></a>Tipo de recurso approvalStage

Namespace: microsoft.graph

Especifica estágios de decisão na aprovação.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|assignedToMe|Booliano|Indica se o estágio é atribuído ao usuário chamador para revisar. Somente leitura.|
|displayName|Cadeia de caracteres|O rótulo fornecido pelo criador da política para identificar um estágio de aprovação. Somente leitura.|
|id|Cadeia de caracteres|O identificador do estágio associado a um objeto de aprovação. Apenas leitura.|
|justification|String|A justificativa associada à decisão do estágio de aprovação.|
|reviewResult|Cadeia de caracteres|O resultado desse registro de aprovação. Os valores possíveis `NotReviewed` incluem: `Approved` , , `Denied` .|
|reviewedBy|[userIdentity](useridentity.md) | O identificador do revistor. Apenas leitura.|
|reviewedDateTime|DateTimeOffset|A data e a hora em que uma decisão foi registrada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|status|Cadeia de caracteres|O status do estágio. Valores possíveis: `InProgress` `Initializing` , , , `Completed` `Expired` . Somente leitura.|

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
