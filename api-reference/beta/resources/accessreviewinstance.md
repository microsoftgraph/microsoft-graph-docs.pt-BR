---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 20d766b61f0de71f36dadac4b9395250fa42214b
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226768"
---
# <a name="accessreviewinstance-resource-type"></a>Tipo de recurso accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma recorrência de revisão de acesso [do](accessreviewsv2-root.md) Azure AD. Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se recorre terá exatamente uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado na definição de agendamento. Se uma definição de agenda analisar vários grupos, cada grupo terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões](accessreviewinstancedecisionitem.md) que os revisores podem tomar medidas. Há uma decisão por identidade sendo revisada.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Leia as propriedades e as relações de um [objeto accessReviewInstance.](../resources/accessreviewinstance.md) |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReviewInstance. |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um accessReviewInstance. |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar decisões manualmente em um accessReviewInstance. |
|[Decisões de registro em lotes](../api/accessreviewinstance-batchrecorddecisions.md)|Nenhum|Revise lotes de entidades ou recursos em uma chamada.|
|[Redefinir decisões](../api/accessreviewinstance-resetdecisions.md)|Nenhum|Redefine todos os itens de decisão em uma instância para `notReviewed` .|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todas as instâncias em um [determinado accessReviewScheduleDefinition](accessreviewscheduledefinition.md) para o qual o usuário de chamada é o revisor de uma ou mais decisões.|
|[Listar decisões](../api/accessreviewinstance-list-decisions.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obter os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.|
|[Lista pendingAccessReviewInstances (preterido)](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [Coleção accessReviewInstance.](accessreviewinstance.md) | Obter todos os recursos de accessReviewInstance pendentes atribuídos ao usuário de chamada. Este método está sendo preterido e substituído por [filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------------------------------- | :---------- |
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura.|
| erros | [Coleção accessReviewError](accessreviewerror.md)| Coleção de erros em um ciclo de vida da instância de revisão de acesso. Apenas leitura. |
| fallbackReviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Suporta o `$select`.|
| id | String | Identificador exclusivo da instância. Oferece suporte para `$select`. Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** e **instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. Suporta `$select` e `$filter` ( `contains` somente). Apenas leitura. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para começar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura. |
| status | String | Especifica o status de um accessReview. Valores possíveis: `Initializing` , , , , , , e `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Apenas leitura.|
| revisadores   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisadores. Suporta o `$select`. Para exemplos de opções para atribuir revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-scope-concept).|


## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| contactedReviewers   |[Coleção accessReviewReviewer](../resources/accessreviewreviewer.md)| Retorna a coleção de revisadores que foram contatados para concluir essa revisão. Embora as propriedades **reviewers** e **fallbackReviewers** do **accessReviewScheduleDefinition** possam especificar proprietários de grupo ou gerentes como revisores **,** **contactedReviewers** retorna suas identidades individuais. Oferece suporte para `$select`. Somente leitura. |
| definition               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Há exatamente um **accessReviewScheduleDefinition** associado a cada instância. É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição. |
| decisions               |[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Cada usuário revisado em **um accessReviewInstance** tem um item de decisão que representa se foi aprovado, negado ou ainda não revisado. |

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
