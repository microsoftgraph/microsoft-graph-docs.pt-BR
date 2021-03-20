---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e5d9b64faafb7dfe4ec4e6f3487643e62885236a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952807"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma decisão de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão. Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Lista cada accessReviewInstanceDecisionItem para um accessReviewInstance específico. |
|[Listar accessReviewInstanceDecisionItems aguardando aprovação](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico. |
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum | Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision. |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo |  Descrição |
| :---------------| :---- | :---------- |
| id | Cadeia de caracteres | O identificador da decisão. |
| accessReviewId | Cadeia de caracteres | O identificador do pai accessReviewInstance. |
| reviewedBy | [userIdentity](useridentity.md) | O identificador do revistor. |
| reviewedDateTime | DateTimeOffset | O timestamp quando a revisão ocorreu. |
| decision | Cadeia de caracteres | Resultado da revisão. Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` . |
| justification | Cadeia de caracteres | A justificativa da decisão de revisão. |
| appliedBy | [userIdentity](useridentity.md) | O identificador do usuário que aplicou a decisão. |
| appliedDateTime | DateTimeOffset | O timestamp quando a decisão de aprovação foi aplicada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
| applyResult | Cadeia de caracteres | O resultado da aplicação da decisão. Valores possíveis: `NotApplied` , , , ou `Success` `Failed` `NotFound` `NotSupported` . |
| recommendation | Cadeia de caracteres | Uma recomendação gerada pelo sistema para a decisão de aprovação. Valores possíveis: `Approve` `Deny` , ou `NotAvailable` .  |
| destino | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | O destino dessa decisão específica. Os destinos de decisão podem ser de tipos diferentes– cada um com suas próprias propriedades específicas. Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| instância |[accessReviewInstance](accessreviewinstance.md) | Há exatamente um accessReviewInstance associado a cada decisão. A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão é tomada. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "openType": true
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
 "id": "string (identifier)",
 "accessReviewId": "string",
 "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
 },
 "reviewedDateTime": "string (timestamp)",
 "decision": "string",
 "justification": "string",
 "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
 "appliedDateTime": "DateTimeOffset",
 "applyResult": "string",
 "recommendation": "string",
 "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstanceDecisionItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
