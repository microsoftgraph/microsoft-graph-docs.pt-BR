---
title: Tipo de recurso accessReviewInstanceDecisionItem
description: Representa uma decisão sobre um accessReviewInstance.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b853ec2e1e663078998809b1f0a5e0701fc353ec
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698349"
---
# <a name="accessreviewinstancedecisionitem-resource-type"></a>Tipo de recurso accessReviewInstanceDecisionItem

Namespace: microsoft.graph

Representa uma Azure AD [de revisão de acesso](accessreviewsv2-overview.md) em uma instância de uma revisão. Essa decisão é a determinação do acesso de uma identidade a um recurso para um [determinado accessReviewInstance](accessreviewinstance.md). accessReviewInstanceDecisionItem é um tipo aberto e permite que outras propriedades sejam passadas.

Cada item de decisão é gerado pelo sistema com base no [accessReviewInstance pai](accessreviewinstance.md).

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstance-list-decisions.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obtenha uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Retorna os itens de decisão para os quais o usuário chamador é o revistor.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessReviewId|Cadeia de Caracteres|O identificador do pai accessReviewInstance. Oferece suporte para `$select`. Somente leitura.|
|appliedBy|[userIdentity](../resources/useridentity.md)|O identificador do usuário que aplicou a decisão. Somente leitura.|
|appliedDateTime|DateTimeOffset|O carimbo de data/hora quando a decisão de aprovação foi aplicada. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.  Oferece suporte para `$select`. Somente leitura.|
|applyResult|Cadeia de Caracteres|O resultado da aplicação da decisão. Valores possíveis: `New`, `AppliedSuccessfully`, `AppliedWithUnknownFailure`e `ApplyNotSupported``AppliedSuccessfullyButObjectNotFound` . Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura.|
|Decisão|Cadeia de Caracteres|Resultado da revisão. Valores possíveis: `Approve`, `Deny`, `NotReviewed`ou `DontKnow`. Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). |
|id|Cadeia de caracteres| O identificador da decisão. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
|Justificação|Cadeia de Caracteres|Justificativa deixada pelo revisores quando eles decidiram.|
|principal|[identity](../resources/identity.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Essa propriedade representa detalhes da entidade de segurança. Por exemplo, se um item de decisão representa o acesso do usuário "Bob" ao Grupo "Vendas" – a entidade é "Bob" e o recurso é "Vendas". As entidades de segurança podem ser de dois tipos: userIdentity e servicePrincipalIdentity. Oferece suporte para `$select`. Somente leitura.|
|principalLink|Cadeia de caracteres|Um link para o objeto principal. Por exemplo, `https://graph.microsoft.com/v1.0/users/a6c7aecb-cbfd-4763-87ef-e91b4bd509d9`. Somente leitura.|
|Recomendação|Cadeia de caracteres|Uma recomendação gerada pelo sistema para a decisão de aprovação com base na última entrada interativa no locatário. É recomendável aprovar se a entrada estiver dentro de trinta dias após o início da revisão. É recomendável negar se a entrada for maior que trinta dias após o início da revisão. Recomendação não disponível caso contrário. Valores possíveis: `Approve`, `Deny`ou `NoInfoAvailable`. Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura.|
|recurso|[accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md)|Cada item de decisão em uma revisão de acesso representa o acesso de uma entidade de segurança a um recurso. Essa propriedade representa detalhes do recurso. Por exemplo, se um item de decisão representa o acesso do usuário "Bob" ao Grupo "Vendas" – a entidade é Bob e o recurso é "Vendas". Os recursos podem ser de vários tipos. Consulte [accessReviewInstanceDecisionItemResource](../resources/accessreviewinstancedecisionitemresource.md). Somente leitura.|
|resourceLink|Cadeia de Caracteres|Um link para o recurso. Por exemplo, `https://graph.microsoft.com/v1.0/servicePrincipals/c86300f3-8695-4320-9f6e-32a2555f5ff8`. Oferece suporte para `$select`. Somente leitura.|
|reviewedBy|[userIdentity](../resources/useridentity.md)| O identificador do revistor. Oferece suporte para `$select`. Somente leitura.|
|reviewedDateTime|DateTimeOffset| O carimbo de data/hora em que a decisão de revisão ocorreu. Oferece suporte para `$select`. Somente leitura.|

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
