---
title: tipo de recurso de filtro
description: Determina quais objetos devem ser provisionados para o aplicativo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82c52e1feac3dd837eb239279523a7a214f97e6b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218433"
---
# <a name="filter-resource-type"></a><span data-ttu-id="4f5a8-103">tipo de recurso de filtro</span><span class="sxs-lookup"><span data-stu-id="4f5a8-103">filter resource type</span></span>

<span data-ttu-id="4f5a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f5a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f5a8-105">Determina quais objetos devem ser provisionados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-105">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="4f5a8-106">Por exemplo, você pode querer provisionar apenas usuários que estão localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-106">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="4f5a8-107">Quando um filtro de escopo estiver presente, os objetos que não satisfaçam o filtro serão ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-107">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="4f5a8-108">O filtro faz parte do [mapeamento de objetos](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="4f5a8-108">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="4f5a8-109">Ele consiste em vários conjuntos de grupos de filtro e cada grupo de filtro contém uma ou mais cláusulas.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-109">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="4f5a8-110">Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`</span><span class="sxs-lookup"><span data-stu-id="4f5a8-110">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="4f5a8-111">Um objeto é considerado em escopo para o conjunto de grupos (o conjunto de grupos `true`é avaliado como) se qualquer um dos grupos no conjunto for `true`avaliado como.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-111">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="4f5a8-112">Para mais informações, consulte [provisionamento de aplicativo baseado em atributo com filtros de escopo](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="4f5a8-112">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="4f5a8-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f5a8-113">Properties</span></span>
| <span data-ttu-id="4f5a8-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f5a8-114">Property</span></span>     | <span data-ttu-id="4f5a8-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f5a8-115">Type</span></span>   |<span data-ttu-id="4f5a8-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f5a8-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f5a8-117">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="4f5a8-117">categoryFilterGroups</span></span>|<span data-ttu-id="4f5a8-118">coleção de [filtro](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="4f5a8-118">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="4f5a8-119">`*Experimental*`Conjunto de grupos de filtro usado para decidir se o objeto fornecido pertence e deve ser processado como parte desse mapeamento de objeto.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-119">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="4f5a8-120">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção for avaliado como `true` \*.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-120">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="4f5a8-121">grupos</span><span class="sxs-lookup"><span data-stu-id="4f5a8-121">groups</span></span>|<span data-ttu-id="4f5a8-122">coleção de [filtro](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="4f5a8-122">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="4f5a8-123">Conjunto de grupos de filtro usado para decidir se o objeto fornecido está no escopo para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-123">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="4f5a8-124">**Este é o filtro que deve ser usado na maioria dos casos**.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-124">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="4f5a8-125">Se um objeto usado para satisfazer esse filtro em um determinado momento e o objeto ou o filtro tiver sido alterado, de forma que o filtro não seja mais satisfeito, esse objeto \* receberá o provisionamento ".</span><span class="sxs-lookup"><span data-stu-id="4f5a8-125">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="4f5a8-126">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção for avaliado como `true` \*.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-126">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="4f5a8-127">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="4f5a8-127">inputFilterGroups</span></span>|<span data-ttu-id="4f5a8-128">coleção de [filtro](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="4f5a8-128">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="4f5a8-129">`*Experimental*`Conjunto de grupos de filtro usado para filtrar objetos no estágio inicial de lê-los a partir do diretório.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-129">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="4f5a8-130">Se um objeto não satisfizer este filtro, ele não será mais processado.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-130">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="4f5a8-131">Importante compreender é que, se um objeto usado para atender a esse filtro em um determinado momento e o objeto ou o filtro tiver sido alterado para que o filtro não seja mais satisfeito, esse objeto *não será obtido sem provisionamento*.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-131">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="4f5a8-132">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção for avaliado como `true` \*.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-132">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f5a8-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f5a8-133">JSON representation</span></span>

<span data-ttu-id="4f5a8-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f5a8-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
