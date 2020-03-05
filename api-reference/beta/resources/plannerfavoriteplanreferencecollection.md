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
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="2705f-103">tipo de recurso plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="2705f-103">plannerFavoritePlanReferenceCollection resource type</span></span>

<span data-ttu-id="2705f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2705f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2705f-105">O recurso **plannerFavoritePlanReferenceCollection** representa a coleção de referências a planos que são marcados como favoritos por um usuário.</span><span class="sxs-lookup"><span data-stu-id="2705f-105">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="2705f-106">Esse recurso é um tipo aberto e faz parte do objeto [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="2705f-106">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="2705f-107">O nome da propriedade no par propriedade-valor é a ID do plano correspondente; o valor é o objeto [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="2705f-107">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="2705f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2705f-108">Properties</span></span>
<span data-ttu-id="2705f-109">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="2705f-109">You can define the properties of this open type.</span></span> <span data-ttu-id="2705f-110">Os nomes das propriedades `id` são valores dos recursos [plannerPlan](plannerplan.md) e seus valores devem ser objetos [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="2705f-110">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="2705f-111">Para remover um item da lista favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="2705f-111">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2705f-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2705f-112">JSON representation</span></span>

<span data-ttu-id="2705f-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2705f-113">The following is a JSON representation of the resource.</span></span>

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
