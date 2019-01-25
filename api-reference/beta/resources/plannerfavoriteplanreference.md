---
title: tipo de recurso de plannerFavoritePlanReference
description: 'O recurso de **plannerFavoritePlanReference** digite representa uma referência a um plannerPlan que foi marcada como favorita pelo usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77a931a882cc4b01725bd8ceb0ae6bcc721a9013
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518384"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="3429e-103">tipo de recurso de plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="3429e-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3429e-104">O recurso de **plannerFavoritePlanReference** digite representa uma referência a um [plannerPlan](plannerplan.md) que foi marcada como favorita pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="3429e-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="3429e-105">Os clientes devem observar que entradas de **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode acessar ou que foram atualizados com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="3429e-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="3429e-106">É recomendável que os clientes notificar os usuários quando houver discrepâncias e manter as entradas atualizado.</span><span class="sxs-lookup"><span data-stu-id="3429e-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="3429e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3429e-107">Properties</span></span>
| <span data-ttu-id="3429e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3429e-108">Property</span></span>     | <span data-ttu-id="3429e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3429e-109">Type</span></span>   |<span data-ttu-id="3429e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3429e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3429e-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="3429e-111">orderHint</span></span>|<span data-ttu-id="3429e-112">String</span><span class="sxs-lookup"><span data-stu-id="3429e-112">String</span></span>|<span data-ttu-id="3429e-p102">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido em [Como usar dicas de ordem no Planner](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="3429e-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="3429e-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="3429e-115">planTitle</span></span>|<span data-ttu-id="3429e-116">String</span><span class="sxs-lookup"><span data-stu-id="3429e-116">String</span></span>|<span data-ttu-id="3429e-117">Título do plano no momento em que o usuário marcado como um favorito.</span><span class="sxs-lookup"><span data-stu-id="3429e-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="3429e-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3429e-118">JSON representation</span></span>

<span data-ttu-id="3429e-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3429e-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
