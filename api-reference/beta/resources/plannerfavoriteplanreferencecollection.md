---
title: tipo de recurso de plannerFavoritePlanReferenceCollection
description: " o valor é o objeto plannerFavoritePlanReference."
ms.openlocfilehash: 78544e17604a0938cc0e88969e2542fc26bdff1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039245"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>tipo de recurso de plannerFavoritePlanReferenceCollection

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **plannerFavoritePlanReferenceCollection** representa a coleção de referências a planos que são marcados como um favorito por um usuário. Este recurso é um tipo aberto e parte do objeto [plannerUser](planneruser.md) . O nome da propriedade no par de valor da propriedade é a ID do plano correspondente; o valor é o objeto [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .


## <a name="properties"></a>Propriedades
Você pode definir as propriedades desse tipo aberto. Os nomes de propriedade são `id` valores de recursos de [plannerPlan](plannerplan.md) e seus valores devem ser [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objetos. Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.


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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
