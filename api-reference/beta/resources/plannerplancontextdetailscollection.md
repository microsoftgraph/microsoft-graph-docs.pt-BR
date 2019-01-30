---
title: tipo de recurso de plannerPlanContextDetailsCollection
description: " o valor é o objeto plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642937"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="3d011-103">tipo de recurso de plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="3d011-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="3d011-104">O recurso de **plannerPlanContextDetailsCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="3d011-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="3d011-105">Este recurso é um tipo aberto e parte do objeto [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="3d011-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="3d011-106">O nome da propriedade no par de valor da propriedade é um identificador de aplicativo específico do contexto; o valor é o objeto [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="3d011-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="3d011-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d011-107">Properties</span></span>
<span data-ttu-id="3d011-108">Propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d011-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="3d011-109">Nesse caso, o cliente deve usar um identificador distinto que representa o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="3d011-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="3d011-110">Os valores de propriedade devem ser [plannerPlanContextDetails](plannerplancontextdetails.md) objetos.</span><span class="sxs-lookup"><span data-stu-id="3d011-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="3d011-111">Com base nos OData, os nomes de propriedade tipos abertos não podem conter os seguintes caracteres: `.`, `:`, `@`, `%`.</span><span class="sxs-lookup"><span data-stu-id="3d011-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="3d011-112">Esses caracteres precisam ser codificada com o formato de codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="3d011-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="3d011-113">Para remover um item na lista Favoritos, o valor deve ser removido da coleção [plannerPlanContextCollection](plannerplancontextcollection.md) em vez disso, que removerá automaticamente a entrada neste objeto.</span><span class="sxs-lookup"><span data-stu-id="3d011-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
