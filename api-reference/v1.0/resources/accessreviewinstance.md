---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um objeto accessReviewScheduleDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5fe495a689a27f5d7dcd76f9148e51185339bdbe
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698307"
---
# <a name="accessreviewinstance-resource-type"></a>Tipo de recurso accessReviewInstance

Namespace: microsoft.graph

Representa uma Azure AD [recorrência](accessreviewsv2-overview.md) de revisão de acesso. Gerado pelo sistema com base no objeto [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai. Todas as propriedades são somente leitura.

Se a instância fizer parte de uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se repetir terá exatamente uma instância. As instâncias também representam cada recurso exclusivo que está sendo revisado na definição de agendamento. Se uma definição de agenda examinar vários recursos, cada recurso terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões nas](accessreviewinstancedecisionitem.md) qual os revisores podem tomar medidas. Há uma decisão por identidade sendo revisada.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md)|[coleção accessReviewInstance](../resources/accessreviewinstance.md)|Obtenha uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades.|
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Leia as propriedades e as relações de um [objeto accessReviewInstance](../resources/accessreviewinstance.md) .|
|[Atualizar accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Atualize os revisores de [um objeto accessReviewInstance](../resources/accessreviewinstance.md) .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todos os objetos de instância em uma definição para a qual o usuário chamador é o revistor.|
|[Listar revisores contatados](../api/accessreviewinstance-list-contactedreviewers.md)|[coleção accessReviewReviewer](../resources/accessreviewreviewer.md)|Obtenha os revisores que receberam notificações para uma instância de revisão de acesso.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|Nenhum|Envie um lembrete aos revisores de um accessReviewInstance.|
|[stop](../api/accessreviewinstance-stop.md)|Nenhum|Interrompa manualmente um accessReviewInstance.|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|Nenhum| Permite que o usuário chamado aceite a recomendação de decisão para cada NotReviewed accessReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico.|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|Nenhum|Aplique manualmente a decisão em um accessReviewInstance.|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Nenhum|Examine lotes de entidades de segurança ou recursos em uma chamada.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Nenhum|Redefine todos os itens de decisão em uma instância para `notReviewed`|
|[Listar decisões](../api/accessreviewinstance-list-decisions.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obtenha os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura.|
| fallbackReviewers   |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisores é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Oferece suporte para `$select`.|
| id | Cadeia de caracteres | Identificador exclusivo da instância. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** **e instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. Dá `$select` suporte e `$filter` (`contains` somente). Somente leitura. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para iniciar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura. |
| status | Cadeia de caracteres | Especifica o status de um accessReview. Valores possíveis: `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`e `AutoReviewed`. Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura.|
| Revisores   |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisores. Oferece suporte para `$select`. Para obter exemplos de opções para atribuir revisores, consulte Atribuir revisores à sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-scope-concept).|


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Decisões|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Cada entidade de segurança revisada em **um accessReviewInstance** tem um item de decisão que representa se eles foram aprovados, negados ou ainda não revisados.|
| contactedReviewers   |[coleção accessReviewReviewer](../resources/accessreviewreviewer.md)| Retorna a coleção de revisores que foram contatados para concluir esta revisão. Embora as propriedades **reviewers** e **fallbackReviewers** do **accessReviewScheduleDefinition** possam especificar proprietários ou gerentes de grupo como revisores **,** **contactedReviewers** retorna suas identidades individuais. Oferece suporte para `$select`. Somente leitura. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstance",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```
