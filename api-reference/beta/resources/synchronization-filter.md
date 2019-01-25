---
title: Tipo de recurso Filter
description: Determina quais objetos devem ser provisionados para o aplicativo. Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA. Quando um filtro de escopo estiver presente, os objetos que satisfazem o filtro não serão ignorados durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516676"
---
# <a name="filter-resource-type"></a><span data-ttu-id="ce4ea-105">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="ce4ea-105">filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce4ea-106">Determina quais objetos devem ser provisionados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-106">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="ce4ea-107">Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-107">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="ce4ea-108">Quando um filtro de escopo estiver presente, os objetos que satisfazem o filtro não serão ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-108">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="ce4ea-109">Filtro faz parte do [mapeamento do objeto](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="ce4ea-109">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="ce4ea-110">Ele consiste em vários conjuntos de grupos de filtro, e cada grupo de filtro contém uma ou mais cláusulas.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-110">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="ce4ea-111">Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-111">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="ce4ea-112">Um objeto é considerado no escopo para conjunto de grupos (conjunto de grupo é avaliado para `true`) se qualquer um dos grupos no conjunto é avaliada para `true`.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-112">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="ce4ea-113">Para obter mais informações, consulte [aplicativo baseado no atributo provisionamento com filtros de escopo](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="ce4ea-113">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="ce4ea-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce4ea-114">Properties</span></span>
| <span data-ttu-id="ce4ea-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce4ea-115">Property</span></span>     | <span data-ttu-id="ce4ea-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce4ea-116">Type</span></span>   |<span data-ttu-id="ce4ea-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4ea-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce4ea-118">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="ce4ea-118">categoryFilterGroups</span></span>|<span data-ttu-id="ce4ea-119">coleção [filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="ce4ea-119">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="ce4ea-120">`*Experimental*`Filtro de conjunto de grupo usado para decidir se determinados objeto pertence e devem ser processadas como parte desse mapeamento do objeto.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-120">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="ce4ea-121">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção é avaliada para `true` \*.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-121">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="ce4ea-122">Grupos</span><span class="sxs-lookup"><span data-stu-id="ce4ea-122">groups</span></span>|<span data-ttu-id="ce4ea-123">coleção [filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="ce4ea-123">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="ce4ea-124">Filtro usado para decidir se determinados objeto está no escopo de provisionamento do conjunto de grupos.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-124">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="ce4ea-125">**Este é o filtro que deve ser usado na maioria dos casos**.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-125">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="ce4ea-126">Se um objeto usado para atender a esse filtro em um determinado momento e, em seguida, o objeto ou o filtro foi alterado por esse filtro não é mais, satisfeito tal objeto \* irá obter provisionado desprovisionamento ".</span><span class="sxs-lookup"><span data-stu-id="ce4ea-126">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="ce4ea-127">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção é avaliada para `true` \*.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-127">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="ce4ea-128">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="ce4ea-128">inputFilterGroups</span></span>|<span data-ttu-id="ce4ea-129">coleção [filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="ce4ea-129">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="ce4ea-130">`*Experimental*`Filtro de conjunto de grupo usado para filtrar os objetos no estágio inicial de leitura-los do diretório.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-130">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="ce4ea-131">Se um objeto não satisfizerem esse filtro não será mais processado.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-131">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="ce4ea-132">É importante entender é que se um objeto usado para atender a esse filtro em um determinado momento, e, em seguida, o objeto ou o filtro foi alterado isso esse filtro não está mais satisfeito, tais objeto *não sejam provisionados desprovisionamento*.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-132">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="ce4ea-133">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção é avaliada para `true` \*.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-133">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce4ea-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce4ea-134">JSON representation</span></span>

<span data-ttu-id="ce4ea-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce4ea-135">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
