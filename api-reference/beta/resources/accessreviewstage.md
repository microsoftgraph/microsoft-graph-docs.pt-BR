---
title: Tipo de recurso accessReviewStage
description: Representa um estágio de accessReviewInstance.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 53d0fa58f4aa494f1815a1205f45ba2673b9620c
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816148"
---
# <a name="accessreviewstage-resource-type"></a>Tipo de recurso accessReviewStage

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa um estágio de recorrência de revisão de acesso do Azure [AD.](accessreviewsv2-overview.md) Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai tiver definido a propriedade **stageSettings** , [o accessReviewInstance](accessReviewInstance.md) será composto por até três estágios subsequentes. Cada estágio pode ter um conjunto diferente de revisadores que podem agir em decisões de estágio e configurações determinando quais decisões passarão de estágio em estágio.

Cada **accessReviewStage** contém uma lista de [decisões que](accessreviewinstancedecisionitem.md) os revisores podem tomar medidas. Há apenas uma decisão por identidade sendo revisada.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewStages](../api/accessreviewinstance-list-stages.md)|[Coleção accessReviewStage](../resources/accessreviewstage.md)|Obter uma lista dos [objetos accessReviewStage](../resources/accessreviewstage.md) e suas propriedades.|
|[Obter accessReviewStage](../api/accessreviewstage-get.md)|[accessReviewStage](../resources/accessreviewstage.md)|Leia as propriedades e as relações de um [objeto accessReviewStage](../resources/accessreviewstage.md) .|
|[Atualizar accessReviewStage](../api/accessreviewstage-update.md)|[accessReviewStage](../resources/accessreviewstage.md)|Atualize as propriedades de um [objeto accessReviewStage](../resources/accessreviewstage.md) .|
|[stop](../api/accessreviewstage-stop.md)|Nenhum(a)| Pare manualmente um accessReviewStage.|
|[filterByCurrentUser](../api/accessreviewstage-filterbycurrentuser.md)|[Coleção accessReviewStage](../resources/accessreviewstage.md)|Retorna todos os estágios em [um accessReviewInstance](accessReviewInstance.md)  determinado para o qual o usuário de chamada é um revisor.|
|[Listar decisões](../api/accessreviewstage-list-decisions.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obter as decisões tomadas em um accessReviewStage.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|endDateTime|DateTimeOffset|DateTime quando o estágio de revisão está agendado para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Essa propriedade é o total acumulado da **duraçãoInDays** para todos os estágios. Somente leitura. |
|fallbackReviewers|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.|
|id|Cadeia de caracteres|Identificador exclusivo do estágio. Somente leitura.|
|revisadores|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisadores. Para ver exemplos de opções para atribuir revisadores, consulte [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).|
|startDateTime|DateTimeOffset|DateTime quando o estágio de revisão está agendado para começar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |
|status|String|Especifica o status de um accessReviewStage. Valores possíveis: `Initializing`, `NotStarted`, `Starting`, `InProgress`, `Completing`, `Completed`, `AutoReviewing`e `AutoReviewed`. Oferece `$orderby`suporte e `$filter` (`eq` somente). Somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|decisions|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Cada usuário revisado em um accessReviewStage tem um item de decisão representando se eles foram aprovados, negados ou ainda não revisados.|

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

