---
title: tipo de recurso de plannerRecentPlanReferenceCollection
description: O recurso de **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram visualizados recentemente por um usuário. Este recurso é um tipo aberto e parte do objeto plannerUser. O nome da propriedade é a ID do plano correspondente. O valor do par de valor da propriedade é o objeto plannerRecentPlanReference.
localization_priority: Normal
ms.openlocfilehash: e77769cbe3a7e53dce518c73cd7c5228d1077dac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877340"
---
# <a name="plannerrecentplanreferencecollection-resource-type"></a>tipo de recurso de plannerRecentPlanReferenceCollection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
