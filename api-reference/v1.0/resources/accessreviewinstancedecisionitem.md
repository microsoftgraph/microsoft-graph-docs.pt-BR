---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4b29eb37f7088185f64b790a15458fa7b30dd7db185bf04903fabaf8d78d124f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163912"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

Representa uma decisão de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão. Essa decisão representa a determinação do acesso de uma identidade a um recurso para um [determinado accessReviewInstance](accessreviewinstance.md).

Cada item de decisão é gerado pelo sistema com base no [accessReviewInstance pai.](accessreviewinstance.md)

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obter uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Retorna os itens de decisão para os quais o usuário de chamada é o revistor.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessReviewId|Cadeia de caracteres|O identificador do pai accessReviewInstance. Oferece suporte para `$select`. Somente leitura.|
|appliedBy|[userIdentity](../resources/useridentity.md)|O identificador do usuário que aplicou a decisão. Somente leitura.|
|appliedDateTime|DateTimeOffset|O timestamp quando a decisão de aprovação foi aplicada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.  Oferece suporte para `$select`. Somente leitura.|
|applyResult|Cadeia de caracteres|O resultado da aplicação da decisão. Valores possíveis: `New` `AppliedSuccessfully` , , e `AppliedWithUnknownFailure` `AppliedSuccessfullyButObjectNotFound` `ApplyNotSupported` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Apenas leitura.|
|decision|String|Resultado da revisão. Valores possíveis: `Approve` `Deny` , , ou `NotReviewed` `DontKnow` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). |
|id|Cadeia de caracteres| O identificador da decisão. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
|justification|Cadeia de caracteres|Justification left by the reviewer when they made the decision.|
|principal|[identity](../resources/identity.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. Essa propriedade representa detalhes da entidade. Por exemplo, se um item de decisão representa o acesso de Usuário "Bob" ao Grupo "Vendas" - a entidade é "Bob" e o recurso é "Vendas". Os principais podem ser de dois tipos - userIdentity e servicePrincipalIdentity. Oferece suporte para `$select`. Somente leitura.|
|principalLink|String|Um link para o objeto principal. Por exemplo, `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Somente leitura.|
|recommendation|Cadeia de caracteres|Uma recomendação gerada pelo sistema para a decisão de aprovação com base na última indicação interativa para locatário. Recomendamos aprovar se a assinatura estiver dentro de trinta dias após o início da revisão. É recomendável negar se a assinatura for maior do que trinta dias do início da revisão. Recomendação não disponível caso contrário. Valores possíveis: `Approve` `Deny` , ou `NoInfoAvailable` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Somente leitura.|
|recurso|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade a um recurso. Essa propriedade representa detalhes do recurso. Por exemplo, se um item de decisão representa o acesso de Usuário "Bob" ao Grupo "Vendas" - a entidade é Bob e o recurso é "Vendas". Os recursos podem ser de vários tipos. Consulte [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Somente leitura.|
|resourceLink|Cadeia de caracteres|Um link para o recurso. Por exemplo, " https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8 ". Oferece suporte para `$select`. Somente leitura.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| O identificador do revistor. Oferece suporte para `$select`. Somente leitura.|
|reviewedDateTime|DateTimeOffset| O timestamp quando ocorreu a decisão de revisão. Oferece suporte para `$select`. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
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
