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
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="6b342-106">tipo de recurso de plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="6b342-106">plannerRecentPlanReferenceCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b342-107">O recurso de **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram visualizados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="6b342-107">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="6b342-108">Este recurso é um tipo aberto e parte do objeto [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="6b342-108">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="6b342-109">O nome da propriedade é a ID do plano correspondente.</span><span class="sxs-lookup"><span data-stu-id="6b342-109">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="6b342-110">O valor do par de valor da propriedade é o objeto [plannerRecentPlanReference](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="6b342-110">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="6b342-111">Adicionar referências de novas a essa coleção removerá automaticamente as entradas mais antigas quando o tamanho da coleção excede um valor máximo predefinido.</span><span class="sxs-lookup"><span data-stu-id="6b342-111">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="6b342-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b342-112">Properties</span></span>
<span data-ttu-id="6b342-113">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="6b342-113">You can define the properties of this open type.</span></span> <span data-ttu-id="6b342-114">Os nomes de propriedade são `id` valores de recursos de [plannerPlan](plannerplan.md) e seus valores devem ser [plannerRecentPlanReference](plannerrecentplanreference.md) objetos.</span><span class="sxs-lookup"><span data-stu-id="6b342-114">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="6b342-115">Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="6b342-115">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b342-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b342-116">JSON representation</span></span>

<span data-ttu-id="6b342-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b342-117">The following is a JSON representation of the resource.</span></span>

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
