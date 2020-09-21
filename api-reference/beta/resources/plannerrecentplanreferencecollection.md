---
title: tipo de recurso plannerRecentPlanReferenceCollection
description: O recurso **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram exibidos recentemente por um usuário. Esse recurso é um tipo aberto e faz parte do objeto plannerUser. O nome da propriedade é a ID do plano correspondente. O valor no par propriedade-valor é o objeto plannerRecentPlanReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 529552be4497729824ddfb9fa9e84ea82e8ccd0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063999"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>tipo de recurso plannerRecentPlanReferenceCollection

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram exibidos recentemente por um usuário. Esse recurso é um tipo aberto e faz parte do objeto [plannerUser](planneruser.md) . O nome da propriedade é a ID do plano correspondente. O valor no par propriedade-valor é o objeto [plannerRecentPlanReference](plannerrecentplanreference.md) .
Adicionar novas referências a essa coleção removerá automaticamente as entradas mais antigas quando o tamanho da coleção exceder um valor máximo pré-determinado.


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os nomes das propriedades são `id` valores dos recursos [plannerPlan](plannerplan.md) e seus valores devem ser objetos [plannerRecentPlanReference](plannerrecentplanreference.md) . Para remover um item da lista favoritos, defina o valor da propriedade como `null` .


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


