---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10166dc9da512bf74a0b4e5ad97f4797cdf6c317
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159196"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma decisão de revisão de acesso [do](accessreviewsv2-root.md) Azure AD em uma instância de uma análise. Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada [instância de revisão de acesso.](accessreviewinstance.md)

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Lista cada accessReviewInstanceDecisionItem para um accessReviewInstance específico. |
|[Listar aprovação pendente de accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico. |
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada é atribuído a um revisor, chamar o usuário pode registrar uma decisão, corrigindo o objeto de decisão. |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo |  Descrição |
| :---------------| :---- | :---------- |
| id | String | O identificador da decisão. |
| accessReviewId | String | O identificador do accessReviewInstance pai. |
| reviewedBy | [userIdentity](useridentity.md) | O identificador do revistor. |
| reviewedDateTime | DateTimeOffset | DateTime em que a revisão ocorreu. |
| decision | String | Resultado da revisão. Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` . |
| justification | String | A justificativa da decisão de revisão. |
| appliedBy | [userIdentity](useridentity.md) | O identificador do usuário que aplicou a decisão. |
| appliedDateTime | DateTimeOffset | DateTime em que a decisão de aprovação foi aplicada. |
| applyResult | String | O resultado da aplicação da decisão. Valores possíveis: `NotApplied` , , , ou `Success` `Failed` `NotFound` `NotSupported` . |
| recomendação | String | Uma recomendação gerada pelo sistema para a decisão de aprovação. Valores possíveis: `Approve` `Deny` , ou `NotAvailable` .  |
| destino | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | O destino dessa decisão específica. Os destinos de decisão podem ser de tipos diferentes, cada um com suas próprias propriedades específicas. Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| instância |[accessReviewInstance](accessreviewinstance.md) | Há exatamente um accessReviewInstance associado a cada decisão. A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão foi tomada. |


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
