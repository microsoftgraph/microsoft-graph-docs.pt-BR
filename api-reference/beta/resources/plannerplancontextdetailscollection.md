---
title: tipo de recurso plannerPlanContextDetailsCollection
description: " o valor é o objeto plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b8adf130dc925a4d9eb17819acf7b2a670a6c7b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965898"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a><span data-ttu-id="970da-103">tipo de recurso plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="970da-103">plannerPlanContextDetailsCollection resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="970da-104">O recurso **plannerPlanContextDetailsCollection** representa a coleção de contextos externos aos quais um plano está vinculado.</span><span class="sxs-lookup"><span data-stu-id="970da-104">The **plannerPlanContextDetailsCollection** resource represents the collection of external contexts to which a plan is linked.</span></span> <span data-ttu-id="970da-105">Esse recurso é um tipo aberto e faz parte do objeto [plannerPlanDetails](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="970da-105">This resource is an open type and is part of the [plannerPlanDetails](plannerplandetails.md) object.</span></span> <span data-ttu-id="970da-106">O nome da propriedade no par propriedade-valor é um identificador específico do aplicativo do contexto; o valor é o objeto [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="970da-106">The property name in the property-value pair is an app-specific identifier of the context; the value is the [plannerPlanContextDetails](plannerplancontextdetails.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="970da-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="970da-107">Properties</span></span>
<span data-ttu-id="970da-108">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="970da-108">Properties of an open type can be defined by the client.</span></span> <span data-ttu-id="970da-109">Nesse caso, o cliente deve usar um identificador distintivo que representa o contexto externo como o nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="970da-109">In this case, the client should use a distinctive identifier that represents the external context as the property name.</span></span> <span data-ttu-id="970da-110">Os valores de propriedade devem ser objetos [plannerPlanContextDetails](plannerplancontextdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="970da-110">The property values must be [plannerPlanContextDetails](plannerplancontextdetails.md) objects.</span></span> <span data-ttu-id="970da-111">Com base em OData, os nomes de propriedade em tipos abertos não podem conter `.`os `:`seguintes `@`caracteres `%`:,,,.</span><span class="sxs-lookup"><span data-stu-id="970da-111">Based on OData, property names in open types cannot contain the following characters: `.`, `:`, `@`, `%`.</span></span> <span data-ttu-id="970da-112">Esses caracteres precisam ser codificados com o formato de codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="970da-112">These characters need to be encoded with URL encoding format.</span></span> <span data-ttu-id="970da-113">Para remover um item da lista favoritos, o valor precisa ser removido da coleção [plannerPlanContextCollection](plannerplancontextcollection.md) , o que removerá automaticamente a entrada desse objeto.</span><span class="sxs-lookup"><span data-stu-id="970da-113">To remove an item in the favorites list, the value needs to be removed from the [plannerPlanContextCollection](plannerplancontextcollection.md) collection instead, which will automatically remove the entry in this object.</span></span>

## <a name="json-representation"></a><span data-ttu-id="970da-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="970da-114">JSON representation</span></span>
<span data-ttu-id="970da-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="970da-115">The following is a JSON representation of the resource.</span></span>

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
