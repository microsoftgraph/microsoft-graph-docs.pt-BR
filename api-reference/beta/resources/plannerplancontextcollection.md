---
title: Tipo de recurso plannerPlanContextCollection
description: O **recurso plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do objeto plannerPlan. O valor no par de valores de propriedade é o objeto plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b2069fd30ba3beb6150b0fdc5dd5bb0f69956b82
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473595"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="634f5-105">Tipo de recurso plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="634f5-105">plannerPlanContextCollection resource type</span></span>

<span data-ttu-id="634f5-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="634f5-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="634f5-107">O **recurso plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="634f5-107">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="634f5-108">Esse recurso é um tipo aberto e faz parte do [objeto plannerPlan.](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="634f5-108">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="634f5-109">O valor no par de valores de propriedade é o [objeto plannerPlanContext.](plannerplancontext.md)</span><span class="sxs-lookup"><span data-stu-id="634f5-109">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="634f5-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="634f5-110">Properties</span></span>
<span data-ttu-id="634f5-111">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="634f5-111">You can define the properties of this open type.</span></span> <span data-ttu-id="634f5-112">Os valores da propriedade devem ser identificadores distintos que representam o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="634f5-112">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="634f5-113">Os valores da propriedade devem ser [objetos plannerPlanContext.](plannerplancontext.md)</span><span class="sxs-lookup"><span data-stu-id="634f5-113">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="634f5-114">Com base nos requisitos OData, os nomes de propriedades em tipos abertos não podem conter os seguintes caracteres: `.` , , , , `:` `%` `@` `#` .</span><span class="sxs-lookup"><span data-stu-id="634f5-114">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`, `#`.</span></span> <span data-ttu-id="634f5-115">Esses caracteres precisam ser codificados usando codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="634f5-115">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="634f5-116">Para remover um item na lista de favoritos, de definir o valor da propriedade como `null` .</span><span class="sxs-lookup"><span data-stu-id="634f5-116">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="634f5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="634f5-117">JSON representation</span></span>

<span data-ttu-id="634f5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="634f5-118">The following is a JSON representation of the resource.</span></span>

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


