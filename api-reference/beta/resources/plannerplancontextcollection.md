---
title: tipo de recurso de plannerPlanContextCollection
description: O recurso de **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Este recurso é um tipo aberto e parte do objeto plannerPlan. O valor do par de valor da propriedade é o objeto plannerPlanContext.
ms.openlocfilehash: ae17e604bf3d59b7b825fe36a8f93f05d5cc835f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036818"
---
# <a name="plannerplancontextcollection-resource-type"></a><span data-ttu-id="f82a8-105">tipo de recurso de plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="f82a8-105">plannerPlanContextCollection resource type</span></span>

> <span data-ttu-id="f82a8-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f82a8-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f82a8-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f82a8-107">Use of these APIs in production applications is not supported.</span></span>


<span data-ttu-id="f82a8-108">O recurso de **plannerPlanContextCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="f82a8-108">The **plannerPlanContextCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="f82a8-109">Este recurso é um tipo aberto e parte do objeto [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="f82a8-109">This resource is an open type and is part of the [plannerPlan](plannerplan.md) object.</span></span> <span data-ttu-id="f82a8-110">O valor do par de valor da propriedade é o objeto [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="f82a8-110">The value in the property-value pair is the [plannerPlanContext](plannerplancontext.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="f82a8-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f82a8-111">Properties</span></span>
<span data-ttu-id="f82a8-112">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="f82a8-112">You can define the properties of this open type.</span></span> <span data-ttu-id="f82a8-113">Os valores de propriedade devem ser um identificador distinto que representa o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="f82a8-113">The property values should be distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="f82a8-114">Os valores de propriedade devem ser [plannerPlanContext](plannerplancontext.md) objetos.</span><span class="sxs-lookup"><span data-stu-id="f82a8-114">The property values must be [plannerPlanContext](plannerplancontext.md) objects.</span></span> <span data-ttu-id="f82a8-115">Com base nos requisitos de OData, os nomes de propriedade tipos abertos não podem conter os seguintes caracteres: `.`, `:`, `%`, `@`.</span><span class="sxs-lookup"><span data-stu-id="f82a8-115">Based on OData requirements, property names in open types cannot contain the following characters: `.`, `:`, `%`, `@`.</span></span> <span data-ttu-id="f82a8-116">Esses caracteres precisam ser codificada usando a codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="f82a8-116">These characters need to be encoded using URL encoding.</span></span> <span data-ttu-id="f82a8-117">Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="f82a8-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f82a8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f82a8-118">JSON representation</span></span>

<span data-ttu-id="f82a8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f82a8-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
