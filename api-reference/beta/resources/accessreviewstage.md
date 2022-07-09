---
title: Tipo de recurso accessReviewStage
description: Representa um estágio de um accessReviewInstance.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 20e23693bce96e0e10eb0f173ceb65ee1516a0a8
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698076"
---
# <a name="accessreviewstage-resource-type"></a>Tipo de recurso accessReviewStage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa um estágio de uma recorrência Azure AD [revisão](accessreviewsv2-overview.md) de acesso. Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai tiver definido a propriedade **stageSettings** , [o accessReviewInstance](accessReviewInstance.md) será composto por até três estágios subsequentes. Cada estágio pode ter um conjunto diferente de revisores que podem agir em decisões de estágio e configurações que determinam quais decisões passarão de estágio para estágio.

Cada **accessReviewStage** contém uma lista de [decisões que](accessreviewinstancedecisionitem.md) os revisores podem tomar medidas. Há apenas uma decisão por identidade sendo revisada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewStages](../api/accessreviewinstance-list-stages.md)|[coleção accessReviewStage](../resources/accessreviewstage.md)|Obtenha uma lista dos [objetos accessReviewStage](../resources/accessreviewstage.md) e suas propriedades.|
|[Obter accessReviewStage](../api/accessreviewstage-get.md)|[accessReviewStage](../resources/accessreviewstage.md)|Leia as propriedades e as relações de um [objeto accessReviewStage](../resources/accessreviewstage.md) .|
|[Atualizar accessReviewStage](../api/accessreviewstage-update.md)|[accessReviewStage](../resources/accessreviewstage.md)|Atualize as propriedades de [um objeto accessReviewStage](../resources/accessreviewstage.md) .|
|[stop](../api/accessreviewstage-stop.md)|Nenhum| Pare manualmente um accessReviewStage.|
|[filterByCurrentUser](../api/accessreviewstage-filterbycurrentuser.md)|[coleção accessReviewStage](../resources/accessreviewstage.md)|Retorna todos os estágios em um [determinado accessReviewInstance para](accessReviewInstance.md)  o qual o usuário chamador é um revisor.|
|[Listar decisões](../api/accessreviewstage-list-decisions.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obtenha as decisões tomadas em um accessReviewStage.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|endDateTime|DateTimeOffset|DateTime quando o estágio de revisão está agendado para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Essa propriedade é o total cumulativo da **durationInDays para** todos os estágios. Somente leitura. |
|fallbackReviewers|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Essa coleção de escopos de revisores é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.|
|id|Cadeia de caracteres|Identificador exclusivo do estágio. Somente leitura.|
|Revisores|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisores. Para obter exemplos de opções para atribuir revisores, consulte Atribuir revisores à sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-scope-concept).|
|startDateTime|DateTimeOffset|DateTime quando o estágio de revisão está agendado para iniciar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
|status|Cadeia de caracteres|Especifica o status de um accessReviewStage. Valores possíveis: `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`e `AutoReviewed`. Dá `$orderby`suporte e `$filter` (`eq` somente). Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Decisões|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Cada usuário revisado em um accessReviewStage tem um item de decisão que representa se eles foram aprovados, negados ou ainda não revisados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewStage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewStage",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
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

