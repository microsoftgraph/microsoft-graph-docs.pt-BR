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
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a><span data-ttu-id="3df99-103">tipo de recurso de plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="3df99-103">plannerFavoritePlanReferenceCollection resource type</span></span>

> <span data-ttu-id="3df99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3df99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3df99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3df99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3df99-106">O recurso de **plannerFavoritePlanReferenceCollection** representa a coleção de referências a planos que são marcados como um favorito por um usuário.</span><span class="sxs-lookup"><span data-stu-id="3df99-106">The **plannerFavoritePlanReferenceCollection** resource represents the collection of references to plans that are marked as a favorite by a user.</span></span> <span data-ttu-id="3df99-107">Este recurso é um tipo aberto e parte do objeto [plannerUser](planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="3df99-107">This resource is an open type and is part of the [plannerUser](planneruser.md) object.</span></span> <span data-ttu-id="3df99-108">O nome da propriedade no par de valor da propriedade é a ID do plano correspondente; o valor é o objeto [plannerFavoritePlanReference](plannerfavoriteplanreference.md) .</span><span class="sxs-lookup"><span data-stu-id="3df99-108">The property name in the property-value pair is the ID of the corresponding plan; the value is the [plannerFavoritePlanReference](plannerfavoriteplanreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="3df99-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3df99-109">Properties</span></span>
<span data-ttu-id="3df99-110">Você pode definir as propriedades desse tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="3df99-110">You can define the properties of this open type.</span></span> <span data-ttu-id="3df99-111">Os nomes de propriedade são `id` valores de recursos de [plannerPlan](plannerplan.md) e seus valores devem ser [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objetos.</span><span class="sxs-lookup"><span data-stu-id="3df99-111">The property names are `id` values of [plannerPlan](plannerplan.md) resources and their values must be [plannerFavoritePlanReference](plannerfavoriteplanreference.md) objects.</span></span> <span data-ttu-id="3df99-112">Para remover um item na lista de Favoritos, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="3df99-112">To remove an item in the favorites list, set the value of the property to `null`.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3df99-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3df99-113">JSON representation</span></span>

<span data-ttu-id="3df99-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3df99-114">The following is a JSON representation of the resource.</span></span>

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
