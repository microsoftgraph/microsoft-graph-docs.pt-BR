---
title: tipo de recurso de plannerRecentPlanReferenceCollection
description: O recurso de **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram visualizados recentemente por um usuário. Este recurso é um tipo aberto e parte do objeto plannerUser. O nome da propriedade é a ID do plano correspondente. O valor do par de valor da propriedade é o objeto plannerRecentPlanReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e27375e3f2395b3528873d8b83f0b5aa6f48d52e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514989"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>tipo de recurso de plannerRecentPlanReferenceCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso de **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram visualizados recentemente por um usuário. Este recurso é um tipo aberto e parte do objeto [plannerUser](planneruser.md) . O nome da propriedade é a ID do plano correspondente. O valor do par de valor da propriedade é o objeto [plannerRecentPlanReference](plannerrecentplanreference.md) .
Adicionar referências de novas a essa coleção removerá automaticamente as entradas mais antigas quando o tamanho da coleção excede um valor máximo predefinido.


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os nomes de propriedade são `id` valores de recursos de [plannerPlan](plannerplan.md) e seus valores devem ser [plannerRecentPlanReference](plannerrecentplanreference.md) objetos. Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.


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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
