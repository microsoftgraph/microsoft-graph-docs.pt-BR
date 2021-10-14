---
title: Tipo de recurso assignmentReviewSettings
description: O tipo assignmentReviewSettings, usado para a propriedade accessReviewSettings de uma política de atribuição de pacote de acesso, fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso nesta política e com que frequência devem ser revisadas.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7bb8afe847a9ceca9f11a54cc7f9c69a44ac0cde
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/13/2021
ms.locfileid: "60290264"
---
# <a name="assignmentreviewsettings-resource-type"></a>Tipo de recurso assignmentReviewSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a **propriedade accessReviewSettings** de uma política de atribuição [de pacote de acesso.](accesspackageassignmentpolicy.md) Fornece configurações adicionais para selecionar quem deve revisar as atribuições de pacote de acesso nesta política e a frequência com que devem ser revisadas.  

## <a name="properties"></a>Propriedades

Esse tipo tem as seguintes propriedades:

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| accessReviewTimeoutBehavior | [accessReviewTimeoutBehavior](#accessreviewtimeoutbehavior-values) | A decisão padrão a ser aplicada se a solicitação não for revisada dentro do período especificado em **durationInDays**. Os valores possíveis são: `acceptAccessRecommendation` `keepAccess` , , e `removeAccess` `unknownFutureValue` . |
| durationInDays | Int32 | O número de dias em que os revisadores devem fornecer entrada.|
| isAccessRecommendationEnabled | Boolean | Especifica se as recomendações serão exibidas ao revistor. O valor padrão é `true` |
| isApprovalJustificationRequired | Boolean | Especifica se o revistor deve fornecer justificativa para a aprovação. O valor padrão é `true`. |
| isEnabled| Booliano | Se for true, as revisões de acesso serão necessárias para atribuições desta política. |
| recurrenceType | String | O intervalo para recorrência, como `monthly` ou `quarterly` . |
| reviewerType | String | Who deve ser solicitado a fazer a revisão, `Self` ou `Reviewers` . |
| revisadores | [Coleção userSet](userset.md) | Se o reviewerType for , essa coleção especificará os usuários que serão revisadores, por ID ou como membros de um grupo, usando uma coleção `Reviewers` [de singleUser](singleuser.md) e [groupMembers](groupmembers.md). |
| startDateTime | DateTimeOffset | Quando a primeira revisão deve começar. |

### <a name="accessreviewtimeoutbehavior-values"></a>valores accessReviewTimeoutBehavior

| Member | Descrição |
|:---------------|:--------|:----------|
| acceptAccessRecommendation | A decisão de revisão de aceitar recomendações da revisão de acesso para aceitar/remover o acesso ao pacote de acesso. A regra geral para recomendações de AR é se o último usuário entrar por mais de 30 dias, é recomendável remover o acesso a esse usuário. |
| keepAccess | A decisão de revisão é manter o acesso atual. |
| removeAccess | A decisão de revisão é remover o acesso ao pacote de acesso. |
| unknownFutureValue | Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentReviewSettings",
  "isEnabled": "Boolean",
  "recurrenceType": "String",
  "reviewerType": "String",
  "startDateTime": "String (timestamp)",
  "durationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "isAccessRecommendationEnabled": "Boolean",
  "isApprovalJustificationRequired": "Boolean",
  "accessReviewTimeoutBehavior": "String"
}
```


