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
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="ed41b-106">tipo de recurso plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="ed41b-106">plannerRecentPlanReferenceCollection resource type</span></span>

<span data-ttu-id="ed41b-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed41b-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed41b-108">O recurso **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram exibidos recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="ed41b-108">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="ed41b-109">Esse recurso é um tipo aberto e faz parte do objeto [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="ed41b-109">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="ed41b-110">O nome da propriedade é a ID do plano correspondente.</span><span class="sxs-lookup"><span data-stu-id="ed41b-110">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="ed41b-111">O valor no par propriedade-valor é o objeto [plannerRecentPlanReference](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="ed41b-111">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="ed41b-112">Adicionar novas referências a essa coleção removerá automaticamente as entradas mais antigas quando o tamanho da coleção exceder um valor máximo pré-determinado.</span><span class="sxs-lookup"><span data-stu-id="ed41b-112">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="ed41b-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed41b-113">Properties</span></span>
<span data-ttu-id="ed41b-114">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="ed41b-114">You can define the properties of this open type.</span></span> <span data-ttu-id="ed41b-115">Os nomes das propriedades são `id` valores dos recursos [plannerPlan](plannerplan.md) e seus valores devem ser objetos [plannerRecentPlanReference](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="ed41b-115">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="ed41b-116">Para remover um item da lista favoritos, defina o valor da propriedade como `null` .</span><span class="sxs-lookup"><span data-stu-id="ed41b-116">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed41b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed41b-117">JSON representation</span></span>

<span data-ttu-id="ed41b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed41b-118">The following is a JSON representation of the resource.</span></span>

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


