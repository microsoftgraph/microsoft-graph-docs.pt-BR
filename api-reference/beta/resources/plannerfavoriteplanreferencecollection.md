---
title: tipo de recurso plannerFavoritePlanReferenceCollection
description: " o valor é o objeto plannerFavoritePlanReference."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c473d4101a1247420e641b532ea04dfbc1a26d2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572623"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="9eb00-103">tipo de recurso plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9eb00-103">plannerFavoritePlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9eb00-104">O recurso **plannerFavoritePlanReferenceCollection** representa a coleção de referências a planos que são marcados como favoritos por um usuário.</span><span class="sxs-lookup"><span data-stu-id="9eb00-104">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="9eb00-105">Esse recurso é um tipo aberto e faz parte do objeto [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="9eb00-105">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="9eb00-106">O nome da propriedade no par propriedade-valor é a ID do plano correspondente; o valor é o objeto [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="9eb00-106">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="9eb00-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9eb00-107">Properties</span></span>
<span data-ttu-id="9eb00-108">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="9eb00-108">You can define the properties of this open type.</span></span> <span data-ttu-id="9eb00-109">Os nomes das propriedades `id` são valores dos recursos [plannerPlan](plannerplan.md) e seus valores devem ser objetos [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="9eb00-109">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="9eb00-110">Para remover um item da lista favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="9eb00-110">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9eb00-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9eb00-111">JSON representation</span></span>

<span data-ttu-id="9eb00-112">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9eb00-112">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
