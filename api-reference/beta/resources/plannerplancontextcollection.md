---
title: tipo de recurso de plannerPlanContextCollection
description: O recurso de **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Este recurso é um tipo aberto e parte do objeto plannerPlan. O valor do par de valor da propriedade é o objeto plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 3281a7664561ac32c3908ca059209a1b89b4ea7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951807"
---
# <a name="plannerplancontextcollection-resource-type"></a>tipo de recurso de plannerPlanContextCollection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.


O recurso de **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Este recurso é um tipo aberto e parte do objeto [plannerPlan](plannerplan.md) . O valor do par de valor da propriedade é o objeto [plannerPlanContext](plannerplancontext.md) .


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os valores de propriedade devem ser um identificador distinto que representa o contexto externo como o nome da propriedade. Os valores de propriedade devem ser [plannerPlanContext](plannerplancontext.md) objetos. Com base nos requisitos de OData, os nomes de propriedade tipos abertos não podem conter os seguintes caracteres: `.`, `:`, `%`, `@`. Esses caracteres precisam ser codificada usando a codificação de URL. Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
