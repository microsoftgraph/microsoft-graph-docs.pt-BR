---
title: Tipo de recurso userLastSignInRecommendationInsightSetting
description: Nas avaliações de acesso do Azure AD, o userLastSignInRecommendationInsightSetting representa as configurações associadas ao insight que se baseia na última data e hora de entrada do usuário e que é usada para ajudar os revisores a tomar decisões.
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aa1467ee59bbedd4765e2a64c22009e713a7e71a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137242"
---
# <a name="userlastsigninrecommendationinsightsetting-resource-type"></a>tipo de recurso userlastsignInrecommendationinsightsetting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O **userLastSignInRecommendationInsightSetting** permite configurar a última data e hora de entrada de um usuário como um insight para ajudar os revisores a tomar decisões para um [objeto accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Herda [de accessReviewRecommendationInsightSetting](accessReviewRecommendationInsightSetting.md).

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| recommendationLookBackDuration | Duração | Opcional. Indica o período de inatividade (em relação à data de início da instância de revisão) de onde as recomendações serão configuradas. A recomendação será para `deny` se o usuário estiver inativo durante a duração do retorno. Para análises de grupos e funções do Azure AD, qualquer duração é aceita. Para análises de aplicativos, 30 dias é a duração máxima. Se não for especificado, a duração será de 30 dias. |
| signInScope | userSignInRecommendationScope | Indica se a inatividade é calculada com base na inatividade do usuário no locatário ou no aplicativo. Os valores possíveis são `tenant` `application` , , `unknownFutureValue` . `application` só é relevante quando a revisão de acesso é uma revisão de uma atribuição a um aplicativo. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userLastSignInRecommendationInsightSetting",
  "baseType": "microsoft.graph.accessReviewRecommendationInsightSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userlastsignInrecommendationinsightsetting",
  "recommendationLookBackDuration": "Duration",
  "signInScope": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "userlastsignInrecommendationinsightsetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
