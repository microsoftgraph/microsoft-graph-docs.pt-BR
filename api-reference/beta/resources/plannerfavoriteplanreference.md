---
title: tipo de recurso de plannerFavoritePlanReference
description: 'O recurso de **plannerFavoritePlanReference** digite representa uma referência a um plannerPlan que foi marcada como favorita pelo usuário. '
localization_priority: Normal
ms.openlocfilehash: b17846eaa1b9a9859d23735d18a191cae4872542
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871320"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="1cdf5-103">tipo de recurso de plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="1cdf5-103">plannerFavoritePlanReference resource type</span></span>

> <span data-ttu-id="1cdf5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cdf5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1cdf5-106">O recurso de **plannerFavoritePlanReference** digite representa uma referência a um [plannerPlan](plannerplan.md) que foi marcada como favorita pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-106">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="1cdf5-107">Os clientes devem observar que entradas de **plannerFavoritePlanReference** podem fazer referência a **plannerPlans** que são excluídas, que o usuário não pode acessar ou que foram atualizados com um título diferente.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-107">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="1cdf5-108">É recomendável que os clientes notificar os usuários quando houver discrepâncias e manter as entradas atualizado.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-108">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="1cdf5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cdf5-109">Properties</span></span>
| <span data-ttu-id="1cdf5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cdf5-110">Property</span></span>     | <span data-ttu-id="1cdf5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cdf5-111">Type</span></span>   |<span data-ttu-id="1cdf5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cdf5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cdf5-113">orderHint</span><span class="sxs-lookup"><span data-stu-id="1cdf5-113">orderHint</span></span>|<span data-ttu-id="1cdf5-114">String</span><span class="sxs-lookup"><span data-stu-id="1cdf5-114">String</span></span>|<span data-ttu-id="1cdf5-p103">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido em [Como usar dicas de ordem no Planner](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="1cdf5-p103">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="1cdf5-117">planTitle</span><span class="sxs-lookup"><span data-stu-id="1cdf5-117">planTitle</span></span>|<span data-ttu-id="1cdf5-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cdf5-118">String</span></span>|<span data-ttu-id="1cdf5-119">Título do plano no momento em que o usuário marcado como um favorito.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-119">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1cdf5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cdf5-120">JSON representation</span></span>

<span data-ttu-id="1cdf5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cdf5-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
