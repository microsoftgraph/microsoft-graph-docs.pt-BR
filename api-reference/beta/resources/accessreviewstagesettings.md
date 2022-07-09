---
title: Tipo de recurso accessReviewStageSettings
description: Em Azure AD revisões de acesso, accessReviewStageSettings representa as configurações dos estágios associados a uma revisão de acesso de vários estágios.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8a7e0142f7f97f608544bc4ca4fc56ab4d3f11dd
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697831"
---
# <a name="accessreviewstagesettings-resource-type"></a>Tipo de recurso accessReviewStageSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa as configurações dos estágios associados a um [objeto de](accessreviewscheduledefinition.md) revisão de acesso de vários estágios. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|decisionsThatWillMoveToNextStage|String collection|Indique quais decisões passarão para o próximo estágio. Pode ser um subconjunto de `Approve`, `Deny`ou `Recommendation``NotReviewed`. Se não for fornecido, todas as decisões passarão para o próximo estágio. Opcional. |
|Dependson|String collection| Define a ordem sequencial ou paralela dos estágios e depende da **stageId**. No momento, há suporte apenas para estágios sequenciais. Por exemplo, se **stageId** for `2`, **dependsOn** deverá ser `1`. Se **stageId** for `1`, não especifique **dependsOn**. Necessário se **stageId** não for `1`. |
|durationInDays|Int32|A duração do estágio. Obrigatório.  <br/><br/>**NOTA:** O valor cumulativo dessa propriedade em todos os estágios <br/> 1. Substituirá a [configuração instanceDurationInDays](accessReviewScheduleSettings.md) no [objeto accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) . <br/>2. Não é possível exceder o comprimento de uma recorrência. Ou seja, se a revisão se repetir semanalmente, a duração **cumulativaInDays** não poderá exceder 7. |
|fallbackReviewers|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Se fornecido, os revisores de fallback serão solicitados a concluir uma revisão se os revisores primários não existirem. Por exemplo, se os gerentes forem  selecionados como revisores e uma entidade de segurança sob revisão não tiver um gerente no Azure AD, os revisores de fallback serão solicitados a examinar essa entidade de segurança. <br/><br/>**NOTA:** O valor dessa propriedade substituirá a configuração correspondente no [objeto accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) .|
|recommendationsEnabled|Booleano|Indica se a exibição de recomendações para revisores está habilitada. Obrigatório. <br/><br/>**NOTA:** O valor dessa propriedade substituirá a configuração [correspondente](accessReviewScheduleSettings.md) no [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .|
| recommendationInsightsSettings | [coleção accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md) | Determina quais recomendações mostrar aos revisores. <br/><br/>**NOTA:** O valor dessa propriedade substituirá a configuração [correspondente](accessReviewScheduleSettings.md) no [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .|
| recommendationLookBackDuration | Duração| Campo opcional. Indica o período de tempo de inatividade (em relação à data de início da instância de revisão) do qual as recomendações serão configuradas. A recomendação será se o `deny` usuário estiver inativo durante a duração do olhar para trás. Para revisões de grupos e Azure AD funções, qualquer duração é aceita. Para revisões de aplicativos, 30 dias é a duração máxima. Se não for especificado, a duração será de 30 dias. <br/><br/>**NOTA:** O valor dessa propriedade substituirá a configuração [correspondente](accessReviewScheduleSettings.md) no [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . |
|Revisores|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Define quem são os revisores. Se nenhum for especificado, a revisão será uma auto-revisão (os usuários revisam seu próprio acesso).  Para obter exemplos de opções para atribuir revisores, consulte Atribuir revisores à sua definição de revisão de acesso [usando o Microsoft API do Graph](/graph/accessreviews-reviewers-concept). <br/><br/>**NOTA:** O valor dessa propriedade substituirá a configuração correspondente em [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md). |
|stageId|Cadeia de Caracteres|Identificador exclusivo do **accessReviewStageSettings**. A **stageId** será usada na **propriedade dependsOn** para indicar a relação de estágio. Obrigatório. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewStageSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewStageSettings",
  "stageId": "String",
  "dependsOn": [
    "String"
  ],
  "durationInDays": "Integer",
  "recommendationsEnabled": "Boolean",
  "recommendationLookBackDuration": "String (duration)",
  "decisionsThatWillMoveToNextStage": [
    "String"
  ],
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

