---
title: tipo de recurso plannerFavoritePlanReference
description: 'O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um plannerPlan que foi marcado como favorito pelo usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 239376a9d1cb8a761cc8f479ff600519b01effcb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344491"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="92bbe-103">tipo de recurso plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="92bbe-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92bbe-104">O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um [plannerPlan](plannerplan.md) que foi marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="92bbe-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="92bbe-105">Os clientes devem observar que as entradas do **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que foram excluídas, que o usuário não pode mais acessar ou que foram atualizadas com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="92bbe-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="92bbe-106">Recomendamos que os clientes Notifiquem os usuários quando houver discrepâncias e mantenha as entradas atualizadas.</span><span class="sxs-lookup"><span data-stu-id="92bbe-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="92bbe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="92bbe-107">Properties</span></span>
| <span data-ttu-id="92bbe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92bbe-108">Property</span></span>     | <span data-ttu-id="92bbe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="92bbe-109">Type</span></span>   |<span data-ttu-id="92bbe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="92bbe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92bbe-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="92bbe-111">orderHint</span></span>|<span data-ttu-id="92bbe-112">String</span><span class="sxs-lookup"><span data-stu-id="92bbe-112">String</span></span>|<span data-ttu-id="92bbe-113">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="92bbe-113">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="92bbe-114">O formato é definido em [usando dicas de ordenação no Planner](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="92bbe-114">The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="92bbe-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="92bbe-115">planTitle</span></span>|<span data-ttu-id="92bbe-116">String</span><span class="sxs-lookup"><span data-stu-id="92bbe-116">String</span></span>|<span data-ttu-id="92bbe-117">Título do plano no momento em que o usuário o marcou como favorito.</span><span class="sxs-lookup"><span data-stu-id="92bbe-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="92bbe-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="92bbe-118">JSON representation</span></span>

<span data-ttu-id="92bbe-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="92bbe-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
