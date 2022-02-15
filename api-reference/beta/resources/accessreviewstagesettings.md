---
title: Tipo de recurso accessReviewStageSettings
description: Em avaliações de acesso do Azure AD, accessReviewStageSettings representa as configurações dos estágios associados a uma revisão de acesso em vários estágios.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: daa7b139aa5a9321965bfe6391c92c16fbc52ffc
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816132"
---
# <a name="accessreviewstagesettings-resource-type"></a>Tipo de recurso accessReviewStageSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa as configurações dos estágios associados a um [objeto de](accessreviewscheduledefinition.md) revisão de acesso de vários estágios. 

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|decisionsThatWillMoveToNextStage|String collection|Indique quais decisões irão para o próximo estágio. Pode ser um sub-conjunto de `Approve`, `Deny`ou `Recommendation``NotReviewed`. Se não for fornecido, todas as decisões passarão para o próximo estágio. Opcional. |
|dependsOn|String collection| Define a ordem sequencial ou paralela dos estágios e depende do **stageId**. No momento, há suporte apenas para estágios sequenciais. Por exemplo, se **stageId** for `2`, **então dependsOn** deve ser `1`. Se **stageId** for `1`, não especifique **dependsOn**. Obrigatório se **stageId** não for `1`. |
|durationInDays|Int32|A duração do estágio. Obrigatório.  <br/><br/>**OBSERVAÇÃO:** O valor acumulado dessa propriedade em todos os estágios <br/> 1. Substituirá a [configuração instanceDurationInDays](accessReviewScheduleSettings.md) no [objeto accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) . <br/>2. Não é possível exceder o comprimento de uma recorrência. Ou seja, se a revisão se recorrência semanal, a duração **cumulativaInDays** não poderá exceder 7. |
|fallbackReviewers|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Se fornecido, os revisadores de fallback serão solicitados a concluir uma revisão se os revistores primários não existirem. Por exemplo, se os gerentes forem  selecionados como revistores e uma entidade em revisão não tiver um gerente no Azure AD, os revisadores de fallback serão solicitados a revisar essa entidade. <br/><br/>**OBSERVAÇÃO:** O valor dessa propriedade substituirá a configuração correspondente no [objeto accessReviewScheduleDefinition](accessReviewScheduleDefinition.md) .|
|recommendationsEnabled|Booliano|Indica se a exibição de recomendações para revisadores está habilitada. Obrigatório. <br/><br/>**OBSERVAÇÃO:** O valor dessa propriedade substituirá a configuração [correspondente no](accessReviewScheduleSettings.md) [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .|
| recommendationInsightsSettings | [coleção accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md) | Determina quais recomendações mostrar aos revisadores. <br/><br/>**OBSERVAÇÃO:** O valor dessa propriedade substituirá a configuração [correspondente no](accessReviewScheduleSettings.md) [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .|
| recommendationLookBackDuration | Duration| Campo opcional. Indica o período de inatividade (em relação à data de início da instância de revisão) de onde as recomendações serão configuradas. A recomendação será para se `deny` o usuário estiver inativo durante a duração de retorno. Para análises de grupos e funções do Azure AD, qualquer duração é aceita. Para análises de aplicativos, 30 dias é a duração máxima. Se não for especificado, a duração será de 30 dias. <br/><br/>**OBSERVAÇÃO:** O valor dessa propriedade substituirá a configuração [correspondente no](accessReviewScheduleSettings.md) [objeto accessReviewScheduleDefinition](accessreviewscheduledefinition.md) . |
|revisadores|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Define quem são os revisadores. Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisam seu próprio acesso).  Para ver exemplos de opções para atribuir revisadores, consulte [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept). <br/><br/>**OBSERVAÇÃO:** O valor dessa propriedade substituirá a configuração correspondente no [accessReviewScheduleDefinition](accessReviewScheduleDefinition.md). |
|stageId|String|Identificador exclusivo do **accessReviewStageSettings**. O **stageId** será usado na **propriedade dependsOn** para indicar a relação de estágio. Obrigatório. |

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

