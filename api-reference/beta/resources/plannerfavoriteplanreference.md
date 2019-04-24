---
title: tipo de recurso plannerFavoritePlanReference
description: 'O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um plannerPlan que foi marcado como favorito pelo usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77a931a882cc4b01725bd8ceb0ae6bcc721a9013
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457095"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="2c511-103">tipo de recurso plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="2c511-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c511-104">O tipo de recurso **plannerFavoritePlanReference** representa uma referência a um [plannerPlan](plannerplan.md) que foi marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="2c511-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="2c511-105">Os clientes devem observar que as entradas do **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que foram excluídas, que o usuário não pode mais acessar ou que foram atualizadas com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="2c511-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="2c511-106">Recomendamos que os clientes Notifiquem os usuários quando houver discrepâncias e mantenha as entradas atualizadas.</span><span class="sxs-lookup"><span data-stu-id="2c511-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="2c511-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c511-107">Properties</span></span>
| <span data-ttu-id="2c511-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c511-108">Property</span></span>     | <span data-ttu-id="2c511-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c511-109">Type</span></span>   |<span data-ttu-id="2c511-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c511-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c511-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="2c511-111">orderHint</span></span>|<span data-ttu-id="2c511-112">String</span><span class="sxs-lookup"><span data-stu-id="2c511-112">String</span></span>|<span data-ttu-id="2c511-113">Dica usada para ordenar itens desse tipo em um modo de exibição de lista.</span><span class="sxs-lookup"><span data-stu-id="2c511-113">Hint used to order items of this type in a list view.</span></span> <span data-ttu-id="2c511-114">O formato é definido em [usando dicas de ordenação no Planner](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="2c511-114">The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="2c511-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="2c511-115">planTitle</span></span>|<span data-ttu-id="2c511-116">String</span><span class="sxs-lookup"><span data-stu-id="2c511-116">String</span></span>|<span data-ttu-id="2c511-117">Título do plano no momento em que o usuário o marcou como favorito.</span><span class="sxs-lookup"><span data-stu-id="2c511-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2c511-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c511-118">JSON representation</span></span>

<span data-ttu-id="2c511-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c511-119">The following is a JSON representation of the resource.</span></span>

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
