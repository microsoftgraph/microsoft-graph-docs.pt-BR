---
title: tipo de recurso de plannerFavoritePlanReference
description: 'O recurso de **plannerFavoritePlanReference** digite representa uma referência a um plannerPlan que foi marcada como favorita pelo usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 48dabeb83522c4151f9da2db9192c7ad546a9bc8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938269"
---
# <a name="plannerfavoriteplanreference-resource-type"></a>tipo de recurso de plannerFavoritePlanReference

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **plannerFavoritePlanReference** digite representa uma referência a um [plannerPlan](plannerplan.md) que foi marcada como favorita pelo usuário. Os clientes devem observar que entradas de **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode acessar ou que foram atualizados com um título diferente.

É recomendável que os clientes notificar os usuários quando houver discrepâncias e manter as entradas atualizado.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|orderHint|String|Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido em [Como usar dicas de ordem no Planner](planner-order-hint-format.md).|
|planTitle|Cadeia de caracteres|Título do plano no momento em que o usuário marcado como um favorito.|


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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
