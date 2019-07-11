---
title: tipo de recurso de filtro
description: Determina quais objetos devem ser provisionados para o aplicativo. Por exemplo, você pode querer provisionar apenas usuários que estão localizados nos EUA. Quando um filtro de escopo estiver presente, os objetos que não satisfaçam o filtro serão ignorados durante a sincronização.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c350216d4d323d736b7d1e3f88234ca206a8116
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621405"
---
# <a name="filter-resource-type"></a><span data-ttu-id="497c7-105">tipo de recurso de filtro</span><span class="sxs-lookup"><span data-stu-id="497c7-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="497c7-106">Determina quais objetos devem ser provisionados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="497c7-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="497c7-107">Por exemplo, você pode querer provisionar apenas usuários que estão localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="497c7-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="497c7-108">Quando um filtro de escopo estiver presente, os objetos que não satisfaçam o filtro serão ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="497c7-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="497c7-109">O filtro faz parte do [mapeamento de objetos](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="497c7-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="497c7-110">Ele consiste em vários conjuntos de grupos de filtro e cada grupo de filtro contém uma ou mais cláusulas.</span><span class="sxs-lookup"><span data-stu-id="497c7-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="497c7-111">Um objeto é considerado no escopo do grupo (o grupo é avaliado como `true`) somente se todas as cláusulas do grupo são avaliadas. `true`</span><span class="sxs-lookup"><span data-stu-id="497c7-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="497c7-112">Um objeto é considerado em escopo para o conjunto de grupos (o conjunto de grupos `true`é avaliado como) se qualquer um dos grupos no conjunto for `true`avaliado como.</span><span class="sxs-lookup"><span data-stu-id="497c7-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="497c7-113">Para mais informações, consulte [provisionamento de aplicativo baseado em atributo com filtros de escopo](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="497c7-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="497c7-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="497c7-114">Properties</span></span>
| <span data-ttu-id="497c7-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="497c7-115">Property</span></span>     | <span data-ttu-id="497c7-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="497c7-116">Type</span></span>   |<span data-ttu-id="497c7-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="497c7-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="497c7-118">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="497c7-118">categoryFilterGroups</span></span>|<span data-ttu-id="497c7-119">coleção de [filtro](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="497c7-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="497c7-120">`*Experimental*`Conjunto de grupos de filtro usado para decidir se o objeto fornecido pertence e deve ser processado como parte desse mapeamento de objeto.</span><span class="sxs-lookup"><span data-stu-id="497c7-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="497c7-121">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção for avaliado como `true` \*.</span><span class="sxs-lookup"><span data-stu-id="497c7-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="497c7-122">grupos</span><span class="sxs-lookup"><span data-stu-id="497c7-122">groups</span></span>|<span data-ttu-id="497c7-123">coleção de [filtro](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="497c7-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="497c7-124">Conjunto de grupos de filtro usado para decidir se o objeto fornecido está no escopo para provisionamento.</span><span class="sxs-lookup"><span data-stu-id="497c7-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="497c7-125">**Este é o filtro que deve ser usado na maioria dos casos**.</span><span class="sxs-lookup"><span data-stu-id="497c7-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="497c7-126">Se um objeto usado para satisfazer esse filtro em um determinado momento e o objeto ou o filtro tiver sido alterado, de forma que o filtro não seja mais satisfeito, esse objeto \* receberá o provisionamento ".</span><span class="sxs-lookup"><span data-stu-id="497c7-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="497c7-127">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção for avaliado como `true` \*.</span><span class="sxs-lookup"><span data-stu-id="497c7-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="497c7-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="497c7-128">inputFilterGroups</span></span>|<span data-ttu-id="497c7-129">coleção de [filtro](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="497c7-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="497c7-130">`*Experimental*`Conjunto de grupos de filtro usado para filtrar objetos no estágio inicial de lê-los a partir do diretório.</span><span class="sxs-lookup"><span data-stu-id="497c7-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="497c7-131">Se um objeto não satisfizer este filtro, ele não será mais processado.</span><span class="sxs-lookup"><span data-stu-id="497c7-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="497c7-132">Importante compreender é que, se um objeto usado para atender a esse filtro em um determinado momento e o objeto ou o filtro tiver sido alterado para que o filtro não seja mais satisfeito, esse objeto *não será obtido sem provisionamento*.</span><span class="sxs-lookup"><span data-stu-id="497c7-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="497c7-133">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção for avaliado como `true` \*.</span><span class="sxs-lookup"><span data-stu-id="497c7-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="497c7-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="497c7-134">JSON representation</span></span>

<span data-ttu-id="497c7-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="497c7-135">Here is a JSON representation of the resource.</span></span>

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
