---
title: tipo complexo accessPackageAssignmentReviewSettings
description: Usado para as avaliações de acesso das atribuições de um pacote de acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8deb20e147d9572911bc94aaec83750e8972592e
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608265"
---
# <a name="accesspackageassignmentreviewsettings-complex-type"></a>tipo complexo accessPackageAssignmentReviewSettings

Namespace: microsoft.graph

Configurações configurada em uma política [de atribuição](accesspackageassignmentpolicy.md) de pacote de acesso para as revisões de acesso de atribuições a um pacote de acesso que foram feitas por meio dessa política. Fornece configurações para selecionar revisadores dessas atribuições e a frequência com que as atribuições devem ser revisadas.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|expirationBehavior|accessReviewExpirationBehavior|A decisão padrão a ser aplicada se o acesso não for revisado. Os valores possíveis são: `keepAccess`, `removeAccess`, `acceptAccessRecommendation`, `unknownFutureValue`.|
|fallbackReviewers|[coleção subjectSet](../resources/subjectset.md)|Essa coleção especifica os usuários que serão os revisadores de fallback quando os revistores primários não responderem.|
|isEnabled|Booliano|If `true`, as avaliações de acesso são necessárias para atribuições por meio desta política.|
|isRecommendationEnabled|Booliano|Especifica se as recomendações serão exibidas ao revistor. O valor padrão é `true`.|
|isReviewerJustificationRequired|Booliano|Especifica se o revistor deve fornecer justificativa para a aprovação. O valor padrão é `true`.|
|isSelfReview|Booliano|Especifica se as entidades de entidades podem revisar suas próprias atribuições.|
|primaryReviewers|[coleção subjectSet](../resources/subjectset.md)|Esta coleção especifica os usuários ou grupo de usuários que revisarão as atribuições do pacote de acesso.|
|Cronograma|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|Quando a primeira revisão deve começar e com que frequência ela deve ser recorrência.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentReviewSettings",
  "isEnabled": "Boolean",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  },
  "isSelfReview": "Boolean",
  "primaryReviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser"
    }
  ],
  "expirationBehavior": "String",
  "isRecommendationEnabled": "Boolean",
  "isReviewerJustificationRequired": "Boolean"
}
```


