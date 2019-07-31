---
title: tipo de recurso plannerPlanContextCollection
description: O recurso **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do objeto plannerPlan. O valor no par propriedade-valor é o objeto plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 34fecf604b68fe092e1feeac2c0e99cc0d59cd77
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965919"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="f0a3d-105">tipo de recurso plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="f0a3d-105">plannerPlanContextCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="f0a3d-106">O recurso **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-106">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="f0a3d-107">Esse recurso é um tipo aberto e faz parte do objeto [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="f0a3d-107">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="f0a3d-108">O valor no par propriedade-valor é o objeto [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="f0a3d-108">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="f0a3d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0a3d-109">Properties</span></span>
<span data-ttu-id="f0a3d-110">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-110">You can define the properties of this open type.</span></span> <span data-ttu-id="f0a3d-111">Os valores de propriedade devem ser um identificador distintivo que representa o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-111">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="f0a3d-112">Os valores de propriedade devem ser objetos [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="f0a3d-112">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="f0a3d-113">Com base nos requisitos de OData, os nomes de propriedade em tipos abertos não podem `.`conter `:`os `%`seguintes `@`caracteres:,,,.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-113">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="f0a3d-114">Esses caracteres precisam ser codificados usando a codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-114">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="f0a3d-115">Para remover um item da lista favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0a3d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0a3d-116">JSON representation</span></span>

<span data-ttu-id="f0a3d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0a3d-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextCollection"
}-->

```json
{
  "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
    "@odata.type": "#microsoft.graph.plannerPlanContext",
    "associationType": "Board",
    "createdDateTime": "2015-10-14T00:57:28.4698344Z",
    "displayNameSegments": [
        "Finance Team",
        "Budget Plans"
    ],
    "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
