---
title: tipo de recurso plannerRecentPlanReferenceCollection
description: O recurso **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram exibidos recentemente por um usuário. Esse recurso é um tipo aberto e faz parte do objeto plannerUser. O nome da propriedade é a ID do plano correspondente. O valor no par propriedade-valor é o objeto plannerRecentPlanReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f63c49013ba9e8c194c1c831e8e78f87e9b8814c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521654"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>tipo de recurso plannerRecentPlanReferenceCollection

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram exibidos recentemente por um usuário. Esse recurso é um tipo aberto e faz parte do objeto [plannerUser](planneruser.md) . O nome da propriedade é a ID do plano correspondente. O valor no par propriedade-valor é o objeto [plannerRecentPlanReference](plannerrecentplanreference.md) .
Adicionar novas referências a essa coleção removerá automaticamente as entradas mais antigas quando o tamanho da coleção exceder um valor máximo pré-determinado.


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os nomes das propriedades `id` são valores dos recursos [plannerPlan](plannerplan.md) e seus valores devem ser objetos [plannerRecentPlanReference](plannerrecentplanreference.md) . Para remover um item da lista favoritos, defina o valor da propriedade como `null`.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
}-->

```json
{
  "7oTB5aMIAE2rVo-1N-L7RmQAGX2q": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-02T22:49:46.155Z",
    "planTitle": "Purchase Workflow"
  },
  "iKNMHkk3vEWpSF7F7iZWIGQAAMMw": {
    "@odata.type": "microsoft.graph.plannerRecentPlanReference",
    "lastAccessedDateTime": "2017-12-03T21:59:28.975Z",
    "planTitle": "New Year's Office Party"
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
