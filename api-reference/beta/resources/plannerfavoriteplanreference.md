---
title: tipo de recurso plannerFavoritePlanReference
description: 'O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um plannerPlan que foi marcado como favorito pelo usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d1bb7cb2ac675d558054523e38ba6bde44378568
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521738"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>tipo de recurso plannerFavoritePlanReference

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um [plannerPlan](plannerplan.md) que foi marcado como favorito pelo usuário. Os clientes devem observar que as entradas do **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que foram excluídas, que o usuário não pode mais acessar ou que foram atualizadas com um título diferente.

Recomendamos que os clientes Notifiquem os usuários quando houver discrepâncias e mantenha as entradas atualizadas.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|orderHint|String|Dica usada para ordenar itens desse tipo em um modo de exibição de lista. O formato é definido em [usando dicas de ordenação no Planner](planner-order-hint-format.md).|
|planTitle|String|Título do plano no momento em que o usuário o marcou como favorito.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
