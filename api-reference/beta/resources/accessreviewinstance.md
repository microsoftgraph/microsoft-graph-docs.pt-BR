---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition`.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5dece4ad638758a51e8aa839cbb755ec5b79d6fd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697215"
---
# <a name="accessreviewinstance-resource-type"></a>Tipo de recurso accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma Azure AD [recorrência](accessreviewsv2-overview.md) de revisão de acesso. Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se repetir terá exatamente uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado na definição de agendamento. Se uma definição de agenda examinar vários grupos, cada grupo terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões nas](accessreviewinstancedecisionitem.md) qual os revisores podem tomar medidas. Há uma decisão por identidade sendo revisada.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstances](../api/accessreviewscheduledefinition-list-instances.md) | [coleção accessReviewInstance](accessreviewinstance.md) | Obtenha uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Leia as propriedades e as relações de um [objeto accessReviewInstance](../resources/accessreviewinstance.md) . |
|[Atualizar accessReviewInstance](../api/accessreviewinstance-update.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Atualize os revisores de [um objeto accessReviewInstance](../resources/accessreviewinstance.md) .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todas as instâncias em um [determinado accessReviewScheduleDefinition](accessreviewscheduledefinition.md) para o qual o usuário chamador é o revisor de uma ou mais decisões.|
|[Listar revisores contatados](../api/accessreviewinstance-list-contactedreviewers.md)|[coleção accessReviewReviewer](../resources/accessreviewreviewer.md)|Obtenha os revisores que receberam notificações para uma instância de revisão de acesso.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Nenhum. | Interrompa manualmente um accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário chamado aceite a recomendação de decisão para cada NotReviewed accessReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar decisões manualmente em um accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Nenhum|Examine lotes de entidades de segurança ou recursos em uma chamada.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Nenhum|Redefine todos os itens de decisão em uma instância para `notReviewed`.|
|[Fases da lista](../api/accessreviewinstance-list-stages.md)|[coleção accessReviewStage](../resources/accessreviewstage.md)| Recupere os estágios em uma instância de revisão de acesso de vários estágios.|
|[Listar decisões](../api/accessreviewinstance-list-decisions.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obtenha os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.|
|[Listar pendingAccessReviewInstances (preterido)](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [coleção accessReviewInstance](accessreviewinstance.md) . | Obtenha todos os recursos de accessReviewInstance pendentes atribuídos ao usuário que está chamando. Esse método está sendo preterido e substituído por [filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------------------------------- | :---------- |
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura.|
| erros | [coleção accessReviewError](accessreviewerror.md)| Coleção de erros em um ciclo de vida da instância de revisão de acesso. Somente leitura. |
| fallbackReviewers   |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisores é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Oferece suporte para `$select`.|
| id | Cadeia de caracteres | Identificador exclusivo da instância. Oferece suporte para `$select`. Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** **e instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. Dá `$select` suporte e `$filter` (`contains` somente). Somente leitura. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para iniciar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura. |
| status | Cadeia de caracteres | Especifica o status de um accessReview. Valores possíveis: `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`e `AutoReviewed`. Dá `$select`suporte `$orderby`a , e `$filter` (`eq` somente). Somente leitura.|
| Revisores   |[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisores. Oferece suporte para `$select`. Para obter exemplos de opções para atribuir revisores, consulte Atribuir revisores à sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-scope-concept).|


## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| contactedReviewers   |[coleção accessReviewReviewer](../resources/accessreviewreviewer.md)| Retorna a coleção de revisores que foram contatados para concluir esta revisão. Embora as propriedades **reviewers** e **fallbackReviewers** do **accessReviewScheduleDefinition** possam especificar proprietários ou gerentes de grupo como revisores **,** **contactedReviewers** retorna suas identidades individuais. Oferece suporte para `$select`. Somente leitura. |
| Definição               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Há exatamente um **accessReviewScheduleDefinition** associado a cada instância. É o agendamento pai da instância, em que as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para examinar pela definição. |
|Estágios|[coleção accessReviewStage](accessreviewstage.md)| Se a instância tiver vários estágios, isso retornará a coleção de estágios. Um novo estágio só será criado quando o estágio anterior terminar. A existência, o número e as configurações de estágios em uma instância de revisão são criados com base no [accessReviewStageSettings](accessreviewstagesettings.md) no [accessReviewScheduleDefinition pai](accessreviewscheduledefinition.md). |
| Decisões               |[coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Cada usuário revisado em **um accessReviewInstance** tem um item de decisão que representa se ele foi aprovado, negado ou ainda não revisado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
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
  ],
  "contactedReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewer"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
