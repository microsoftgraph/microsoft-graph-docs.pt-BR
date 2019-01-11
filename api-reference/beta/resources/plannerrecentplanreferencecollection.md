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
# <a name="plannerrecentplanreferencecollection-resource-type"></a><span data-ttu-id="b1c61-106">tipo de recurso de plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="b1c61-106">plannerRecentPlanReferenceCollection resource type</span></span>

> <span data-ttu-id="b1c61-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1c61-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1c61-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1c61-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1c61-109">O recurso de **plannerRecentPlanReferenceCollection** representa a coleção de referências a planos que foram visualizados recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="b1c61-109">The **plannerRecentPlanReferenceCollection** resource represents the collection of references to plans that were recently viewed by a user.</span></span> <span data-ttu-id="b1c61-110">Este recurso é um tipo aberto e parte do objeto [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c61-110">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="b1c61-111">O nome da propriedade é a ID do plano correspondente.</span><span class="sxs-lookup"><span data-stu-id="b1c61-111">The property name is the ID of the corresponding plan.</span></span> <span data-ttu-id="b1c61-112">O valor do par de valor da propriedade é o objeto [plannerRecentPlanReference](plannerrecentplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="b1c61-112">The value in the property-value pair is the [plannerRecentPlanReference](plannerrecentplanreference.md) object.</span></span>
<span data-ttu-id="b1c61-113">Adicionar referências de novas a essa coleção removerá automaticamente as entradas mais antigas quando o tamanho da coleção excede um valor máximo predefinido.</span><span class="sxs-lookup"><span data-stu-id="b1c61-113">Adding new references to this collection will automatically remove the oldest entries when the size of the collection exceeds a predetermined maximum value.</span></span>


## <a name="properties"></a><span data-ttu-id="b1c61-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1c61-114">Properties</span></span>
<span data-ttu-id="b1c61-115">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="b1c61-115">You can define the properties of this open type.</span></span> <span data-ttu-id="b1c61-116">Os nomes de propriedade são `id` valores de recursos de [plannerPlan](plannerplan.md) e seus valores devem ser [plannerRecentPlanReference](plannerrecentplanreference.md) objetos.</span><span class="sxs-lookup"><span data-stu-id="b1c61-116">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerRecentPlanReference](plannerrecentplanreference.md) objects.</span></span> <span data-ttu-id="b1c61-117">Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="b1c61-117">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b1c61-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1c61-118">JSON representation</span></span>

<span data-ttu-id="b1c61-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1c61-119">The following is a JSON representation of the resource.</span></span>

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
