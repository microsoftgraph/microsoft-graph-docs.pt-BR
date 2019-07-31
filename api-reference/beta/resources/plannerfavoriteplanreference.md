---
title: tipo de recurso plannerFavoritePlanReference
description: 'O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um plannerPlan que foi marcado como favorito pelo usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 07803375ca31162f0f7e392d81edb83ab2bd6da3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009066"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="05f12-103">tipo de recurso plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="05f12-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05f12-104">O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um [plannerPlan](plannerplan.md) que foi marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="05f12-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="05f12-105">Os clientes devem observar que as entradas do **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que foram excluídas, que o usuário não pode mais acessar ou que foram atualizadas com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="05f12-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="05f12-106">Recomendamos que os clientes Notifiquem os usuários quando houver discrepâncias e mantenha as entradas atualizadas.</span><span class="sxs-lookup"><span data-stu-id="05f12-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="05f12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05f12-107">Properties</span></span>
| <span data-ttu-id="05f12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05f12-108">Property</span></span>     | <span data-ttu-id="05f12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="05f12-109">Type</span></span>   |<span data-ttu-id="05f12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="05f12-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05f12-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="05f12-111">orderHint</span></span>|<span data-ttu-id="05f12-112">String</span><span class="sxs-lookup"><span data-stu-id="05f12-112">String</span></span>|<span data-ttu-id="05f12-113">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="05f12-113">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="05f12-114">O formato é definido em [usando dicas de ordenação no Planner](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="05f12-114">The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="05f12-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="05f12-115">planTitle</span></span>|<span data-ttu-id="05f12-116">String</span><span class="sxs-lookup"><span data-stu-id="05f12-116">String</span></span>|<span data-ttu-id="05f12-117">Título do plano no momento em que o usuário o marcou como favorito.</span><span class="sxs-lookup"><span data-stu-id="05f12-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="05f12-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05f12-118">JSON representation</span></span>

<span data-ttu-id="05f12-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05f12-119">The following is a JSON representation of the resource.</span></span>

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
