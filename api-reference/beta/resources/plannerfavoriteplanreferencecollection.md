---
title: tipo de recurso plannerFavoritePlanReferenceCollection
description: " o valor é o objeto plannerFavoritePlanReference."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 32c0cecc402570491c0025c0b4e0c88b74ed40fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521731"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>tipo de recurso plannerFavoritePlanReferenceCollection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerFavoritePlanReferenceCollection** representa a coleção de referências a planos que são marcados como favoritos por um usuário. Esse recurso é um tipo aberto e faz parte do objeto [plannerUser](planneruser.md) . O nome da propriedade no par propriedade-valor é a ID do plano correspondente; o valor é o objeto [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os nomes das propriedades `id` são valores dos recursos [plannerPlan](plannerplan.md) e seus valores devem ser objetos [plannerFavoritePlanReference](plannerfavoriteplanreference.md) . Para remover um item da lista favoritos, defina o valor da propriedade como `null`.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
