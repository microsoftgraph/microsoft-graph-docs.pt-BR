---
title: tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9ad5f8a49d44c82f1a43a1666f08f2b49853395
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000779"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma decisão de [revisão](accessreviewsv2-root.md) do Azure ad Access em uma instância de uma revisão. Essa decisão representa a determinação do acesso de um usuário ou de uma entidade de serviço para uma determinada [instância de análise do Access](accessreviewinstance.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Lista todos os accessReviewInstanceDecisionItem para um accessReviewInstance específico. |
|[Listar accessReviewInstanceDecisionItems pendente de aprovação](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Obtenha todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico. |
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer accessReviewInstanceDecisionItems ao qual o usuário de chamada tenha atribuído um revisor, o usuário de chamada pode gravar uma decisão corrigindo o objeto de decisão. |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo |  Descrição |
| :---------------| :---- | :---------- |
| id | Cadeia de caracteres | O identificador da decisão. |
| accessReviewId | Cadeia de caracteres | O identificador do accessReviewInstance pai. |
| reviewedBy | [userIdentity](useridentity.md) | O identificador do revisor. |
| reviewedDateTime | DateTimeOffset | O DateTime quando a revisão ocorreu. |
| sobre | Cadeia de caracteres | Resultado da revisão. Valores possíveis: `Approve` , `Deny` , `NotReviewed` ou `DontKnow` . |
| elabora | Cadeia de caracteres | A justificativa de decisão de revisão. |
| appliedBy | [userIdentity](useridentity.md) | O identificador do usuário que aplicou a decisão. |
| appliedDateTime | DateTimeOffset | O DateTime quando a decisão de aprovação foi aplicada. |
| applyResult | Cadeia de caracteres | O resultado da aplicação da decisão. Valores possíveis: `NotApplied` , `Success` , `Failed` , `NotFound` , ou `NotSupported` . |
| recomendação | Cadeia de caracteres | Uma recomendação gerada pelo sistema para a decisão de aprovação. Valores possíveis: `Approve` , `Deny` , ou `NotAvailable` .  |
| destino | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | O alvo dessa decisão específica. Os alvos de decisão podem ser de tipos diferentes, cada um com suas próprias propriedades específicas. Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| sessão |[accessReviewInstance](accessreviewinstance.md) | Há exatamente um accessReviewInstance associado a cada decisão. A instância é pai do item de decisão, representando a recorrência da revisão do Access na qual a decisão é realizada. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "",
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
