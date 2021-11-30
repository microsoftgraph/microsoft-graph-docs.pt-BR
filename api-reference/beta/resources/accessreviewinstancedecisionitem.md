---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3b8e653c05e428bf0f1dc4efa8e1efb8cb4e2815
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224234"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

>[!NOTE]
>A propriedade `target` será preterida em v1.0 e substituída pelas `principal` propriedades `resource` e.

Representa uma decisão de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão. Essa decisão é a determinação do acesso de um usuário ou entidade de serviço para uma determinada instância de revisão [de acesso.](accessreviewinstance.md) accessReviewInstanceDecisionItem é um tipo aberto e permite que outras propriedades sejam passadas.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Obter uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Recupera todos os [objetos accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) onde o uso de chamada é o revisor de um [dado accessReviewInstance](accessreviewinstance.md).|
|[Listar accessReviewInstanceDecisionItems pendente aprovação (preterida)](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico. Este método está sendo preterido e substituído por [filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo |  Descrição |
| :---------------| :---- | :---------- |
|accessReviewId|Cadeia de Caracteres|O identificador do pai accessReviewInstance. Oferece suporte para `$select`. Somente leitura.|
|appliedBy|[userIdentity](../resources/useridentity.md)|O identificador do usuário que aplicou a decisão. Apenas leitura.|
|appliedDateTime|DateTimeOffset|O timestamp quando a decisão de aprovação foi aplicada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.  Oferece suporte para `$select`. Somente leitura.|
|applyResult|Cadeia de Caracteres|O resultado da aplicação da decisão. Valores possíveis: `New` `AppliedSuccessfully` , , e `AppliedWithUnknownFailure` `AppliedSuccessfullyButObjectNotFound` `ApplyNotSupported` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Apenas leitura.|
|decision|Cadeia de Caracteres|Resultado da revisão. Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). |
|id|String| O identificador da decisão. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
|justification|Cadeia de Caracteres|Justification left by the reviewer when they made the decision.|
| destino | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | O destino dessa decisão específica. Os destinos de decisão podem ser de tipos diferentes– cada um com suas próprias propriedades específicas. Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). Apenas leitura.|
|principal|[identity](../resources/identity.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. Essa propriedade representa detalhes da entidade. Por exemplo, se um item de decisão representa o acesso de Usuário "Bob" ao Grupo "Vendas" - a entidade é "Bob" e o recurso é "Vendas". Os principais podem ser de dois tipos - userIdentity e servicePrincipalIdentity. Oferece suporte para `$select`. Somente leitura.|
|principalLink|Cadeia de Caracteres|Link para o objeto principal. Por exemplo: `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Apenas leitura.|
|recommendation|Cadeia de Caracteres|Uma recomendação gerada pelo sistema para a decisão de aprovação com base na última indicação interativa para locatário. Recomendamos aprovar se a assinatura estiver dentro de trinta dias após o início da revisão. É recomendável negar se a assinatura for maior do que trinta dias do início da revisão. Recomendação não disponível caso contrário. Valores possíveis: `Approve` `Deny` , ou `NoInfoAvailable` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Apenas leitura.|
|recurso|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. Essa propriedade representa detalhes do recurso. Por exemplo, se um item de decisão representa o acesso de Usuário "Bob" ao Grupo "Vendas" - a entidade é Bob e o recurso é "Vendas". Os recursos podem ser de vários tipos. Consulte [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Apenas leitura.|
|resourceLink|Cadeia de Caracteres|Um link para o recurso. Por exemplo, `https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`. Oferece suporte para `$select`. Somente leitura.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| O identificador do revistor. Oferece suporte para `$select`. Somente leitura.|
|reviewedDateTime|DateTimeOffset| O timestamp quando ocorreu a decisão de revisão. Oferece suporte para `$select`. Somente leitura.|

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
  "id": "String (identifier)",
  "accessReviewId": "String",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "reviewedDateTime": "String (timestamp)",
  "decision": "String",
  "justification": "String",
  "appliedBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "appliedDateTime": "String (timestamp)",
  "applyResult": "String",
  "recommendation": "String",
  "target": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemTarget"
  },
  "principal": {
    "@odata.type": "microsoft.graph.identity"
  },
  "principalLink": "String",
  "resource": {
    "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItemResource"
  },
  "resourceLink": "String"
}
```
