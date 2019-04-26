---
title: tipo de recurso plannerPlanContextCollection
description: O recurso **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do objeto plannerPlan. O valor no par propriedade-valor é o objeto plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 8d5394ff8a9503ab9ffba4810c9c2cad0d9a2fbf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344447"
---
# <a name="plannerplancontextcollection-resource-type"></a>tipo de recurso plannerPlanContextCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


O recurso **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do objeto [plannerPlan](plannerplan.md) . O valor no par propriedade-valor é o objeto [plannerPlanContext](plannerplancontext.md) .


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os valores de propriedade devem ser um identificador distintivo que representa o contexto externo como o nome da propriedade. Os valores de propriedade devem ser objetos [plannerPlanContext](plannerplancontext.md) . Com base nos requisitos de OData, os nomes de propriedade em tipos abertos não podem `.`conter `:`os `%`seguintes `@`caracteres:,,,. Esses caracteres precisam ser codificados usando a codificação de URL. Para remover um item da lista favoritos, defina o valor da propriedade como `null`.

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
