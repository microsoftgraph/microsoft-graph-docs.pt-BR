---
title: tipo de recurso plannerPlanContextDetailsCollection
description: " o valor é o objeto plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 2e2f292de763674510f6da5a8aad90fe8e17ab7f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344393"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="2f5f7-103">tipo de recurso plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="2f5f7-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="2f5f7-104">O recurso **plannerPlanContextDetailsCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="2f5f7-105">Esse recurso é um tipo aberto e faz parte do objeto [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="2f5f7-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="2f5f7-106">O nome da propriedade no par propriedade-valor é um identificador específico do aplicativo do contexto; o valor é o objeto [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="2f5f7-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="2f5f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f5f7-107">Properties</span></span>
<span data-ttu-id="2f5f7-108">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="2f5f7-109">Nesse caso, o cliente deve usar um identificador distintivo que representa o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="2f5f7-110">Os valores de propriedade devem ser objetos [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="2f5f7-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="2f5f7-111">Com base em OData, os nomes de propriedade em tipos abertos não podem conter `.`os `:`seguintes `@`caracteres `%`:,,,.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="2f5f7-112">Esses caracteres precisam ser codificados com o formato de codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="2f5f7-113">Para remover um item da lista favoritos, o valor precisa ser removido da coleção [plannerPlanContextCollection](plannerplancontextcollection.md) , o que removerá automaticamente a entrada desse objeto.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f5f7-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f5f7-114">JSON representation</span></span>
<span data-ttu-id="2f5f7-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f5f7-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
