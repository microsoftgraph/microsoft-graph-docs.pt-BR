---
title: Tipo de recurso plannerPlanContextCollection
description: O **recurso plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do objeto plannerPlan. O valor no par de valores de propriedade é o objeto plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b2069fd30ba3beb6150b0fdc5dd5bb0f69956b82
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473595"
---
# <a name="plannerplancontextcollection-resource-type"></a>Tipo de recurso plannerPlanContextCollection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


O **recurso plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do [objeto plannerPlan.](plannerplan.md) O valor no par de valores de propriedade é o [objeto plannerPlanContext.](plannerplancontext.md)


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os valores da propriedade devem ser identificadores distintos que representam o contexto externo como o nome da propriedade. Os valores da propriedade devem ser [objetos plannerPlanContext.](plannerplancontext.md) Com base nos requisitos OData, os nomes de propriedades em tipos abertos não podem conter os seguintes caracteres: `.` , , , , `:` `%` `@` `#` . Esses caracteres precisam ser codificados usando codificação de URL. Para remover um item na lista de favoritos, de definir o valor da propriedade como `null` .

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


