---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre o acesso de um usuário em um accessReviewInstance.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 633e095d0fbb2843c888e52f1d71bb0eda1c4644
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697887"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma Azure AD [de revisão de acesso](accessreviewsv2-overview.md) em uma instância de uma revisão. Essa decisão representa a determinação do acesso de um usuário ou entidade de serviço para uma determinada instância [de revisão de acesso](accessreviewinstance.md).  Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstance-list-decisions.md) | [coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Obtenha uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer accessReviewInstanceDecisionItems ao qual o usuário chamador é atribuído a um revisor, chamar o usuário pode registrar uma decisão aplicando patch ao objeto de decisão. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Recupera todos [os objetos accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) em que o uso de chamada é o revisor de um [determinado accessReviewInstance](accessreviewinstance.md).|
|[Listar accessReviewInstanceDecisionItems com aprovação pendente (preterido)](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Obtenha todos os accessReviewInstanceDecisionItems atribuídos ao usuário chamador para um accessReviewInstance específico. Esse método está sendo preterido e substituído por [filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo |  Descrição |
| :---------------| :---- | :---------- |
|accessReviewId|Cadeia de caracteres|O identificador do pai accessReviewInstance. Oferece suporte para `$select`. Somente leitura.|
|appliedBy|[userIdentity](../resources/useridentity.md)|O identificador do usuário que aplicou a decisão. Somente leitura.|
|appliedDateTime|DateTimeOffset|O carimbo de data/hora quando a decisão de aprovação foi aplicada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.  Oferece suporte para `$select`. Somente leitura.|
|applyResult|Cadeia de Caracteres|O resultado da aplicação da decisão. Valores possíveis: `New`, `AppliedSuccessfully`, `AppliedWithUnknownFailure`e `ApplyNotSupported``AppliedSuccessfullyButObjectNotFound` . Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura.|
|Decisão|Cadeia de Caracteres|Resultado da revisão. Valores possíveis: `Approve`, `Deny`, `NotReviewed`ou `DontKnow`. Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). |
|id|Cadeia de caracteres| O identificador da decisão. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
|Justificação|Cadeia de Caracteres|Justificativa deixada pelo revisores quando eles decidiram.|
| destino | [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md)  | O destino dessa decisão específica. Os destinos de decisão podem ser de tipos diferentes– cada um com suas próprias propriedades específicas. Consulte [accessReviewInstanceDecisionItemTarget](accessreviewinstancedecisionitemtarget.md). Somente leitura. <br/> Essa propriedade foi substituída pelas propriedades `principal` `resource` na v1.0.|
|principal|[identity](../resources/identity.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Essa propriedade representa detalhes da entidade de segurança. Por exemplo, se um item de decisão representa o acesso do usuário "Bob" ao Grupo "Vendas" – a entidade é "Bob" e o recurso é "Vendas". As entidades de segurança podem ser de dois tipos: userIdentity e servicePrincipalIdentity. Oferece suporte para `$select`. Somente leitura.|
|principalLink|Cadeia de Caracteres|Link para o objeto principal. Por exemplo: `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Somente leitura.|
|Recomendação|Cadeia de caracteres|Uma recomendação gerada pelo sistema para a decisão de aprovação com base na última entrada interativa no locatário. É recomendável aprovar se a entrada estiver dentro de trinta dias após o início da revisão. É recomendável negar se a entrada for maior que trinta dias após o início da revisão. Recomendação não disponível caso contrário. Valores possíveis: `Approve`, `Deny`ou `NoInfoAvailable`. Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura.|
|recurso|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Essa propriedade representa detalhes do recurso. Por exemplo, se um item de decisão representa o acesso do usuário "Bob" ao Grupo "Vendas" – a entidade é Bob e o recurso é "Vendas". Os recursos podem ser de vários tipos. Consulte [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Somente leitura.|
|resourceLink|Cadeia de Caracteres|Um link para o recurso. Por exemplo, `https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`. Oferece suporte para `$select`. Somente leitura.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| O identificador do revistor. Oferece suporte para `$select`. Somente leitura.|
|reviewedDateTime|DateTimeOffset| O carimbo de data/hora em que a decisão de revisão ocorreu. Oferece suporte para `$select`. Somente leitura.|
|principalResourceMembership|[decisionItemPrincipalResourceMembership](../resources/decisionItemPrincipalResourceMembership.md)| Cada item de decisão em uma revisão de acesso representa a associação de uma entidade de segurança a um recurso. Essa propriedade fornece os detalhes da associação. Por exemplo, se a entidade de segurança tem acesso direto ou indireto ao recurso. Oferece suporte para `$select`. Somente leitura.|


## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| instância |[accessReviewInstance](accessreviewinstance.md) | Há exatamente um accessReviewInstance associado a cada decisão. A instância é o pai do item de decisão, representando a recorrência da revisão de acesso em que a decisão é tomada. |
| insights |[coleção governanceInsight](governanceinsight.md) | Insights são recomendações para revisores sobre se deseja aprovar ou negar uma decisão. Pode haver vários insights associados a **um accessReviewInstanceDecisionItem**. |


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
  "principalResourceMembership": {
    "@odata.type": "microsoft.graph.decisionItemPrincipalResourceMembership"
  },
  "resourceLink": "String"
}
```
