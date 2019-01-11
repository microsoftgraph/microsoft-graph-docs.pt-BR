---
title: tipo de recurso de filtro
description: Determina quais objetos devem ser provisionados para o aplicativo. Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA. Quando um filtro de escopo estiver presente, os objetos que satisfazem o filtro não serão ignorados durante a sincronização.
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894408"
---
# <a name="filter-resource-type"></a><span data-ttu-id="3da93-105">tipo de recurso de filtro</span><span class="sxs-lookup"><span data-stu-id="3da93-105">filter resource type</span></span>

> <span data-ttu-id="3da93-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3da93-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3da93-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3da93-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3da93-108">Determina quais objetos devem ser provisionados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3da93-108">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="3da93-109">Por exemplo, você talvez queira apenas os usuários de provisão que estão localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="3da93-109">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="3da93-110">Quando um filtro de escopo estiver presente, os objetos que satisfazem o filtro não serão ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="3da93-110">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="3da93-111">Filtro faz parte do [mapeamento do objeto](synchronization-objectmapping.md).</span><span class="sxs-lookup"><span data-stu-id="3da93-111">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="3da93-112">Ele consiste em vários conjuntos de grupos de filtro, e cada grupo de filtro contém uma ou mais cláusulas.</span><span class="sxs-lookup"><span data-stu-id="3da93-112">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="3da93-113">Um objeto é considerado no escopo do grupo (o grupo é avaliado para `true`) somente se todas as cláusulas do grupo são avaliadas para `true`.</span><span class="sxs-lookup"><span data-stu-id="3da93-113">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="3da93-114">Um objeto é considerado no escopo para conjunto de grupos (conjunto de grupo é avaliado para `true`) se qualquer um dos grupos no conjunto é avaliada para `true`.</span><span class="sxs-lookup"><span data-stu-id="3da93-114">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="3da93-115">Para obter mais informações, consulte [aplicativo baseado no atributo provisionamento com filtros de escopo](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="3da93-115">For more information, see [Attribute-based application provisioning with scoping filters](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="3da93-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3da93-116">Properties</span></span>
| <span data-ttu-id="3da93-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3da93-117">Property</span></span>     | <span data-ttu-id="3da93-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="3da93-118">Type</span></span>   |<span data-ttu-id="3da93-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da93-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3da93-120">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="3da93-120">categoryFilterGroups</span></span>|<span data-ttu-id="3da93-121">coleção [filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="3da93-121">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="3da93-122">`*Experimental*`Filtro de conjunto de grupo usado para decidir se determinados objeto pertence e devem ser processadas como parte desse mapeamento do objeto.</span><span class="sxs-lookup"><span data-stu-id="3da93-122">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="3da93-123">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção é avaliada para `true` \*.</span><span class="sxs-lookup"><span data-stu-id="3da93-123">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="3da93-124">grupos</span><span class="sxs-lookup"><span data-stu-id="3da93-124">groups</span></span>|<span data-ttu-id="3da93-125">coleção [filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="3da93-125">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="3da93-126">Filtro usado para decidir se determinados objeto está no escopo de provisionamento do conjunto de grupos.</span><span class="sxs-lookup"><span data-stu-id="3da93-126">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="3da93-127">**Este é o filtro que deve ser usado na maioria dos casos**.</span><span class="sxs-lookup"><span data-stu-id="3da93-127">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="3da93-128">Se um objeto usado para atender a esse filtro em um determinado momento e, em seguida, o objeto ou o filtro foi alterado por esse filtro não é mais, satisfeito tal objeto \* irá obter provisionado desprovisionamento ".</span><span class="sxs-lookup"><span data-stu-id="3da93-128">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="3da93-129">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção é avaliada para `true` \*.</span><span class="sxs-lookup"><span data-stu-id="3da93-129">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="3da93-130">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="3da93-130">inputFilterGroups</span></span>|<span data-ttu-id="3da93-131">coleção [filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="3da93-131">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="3da93-132">`*Experimental*`Filtro de conjunto de grupo usado para filtrar os objetos no estágio inicial de leitura-los do diretório.</span><span class="sxs-lookup"><span data-stu-id="3da93-132">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="3da93-133">Se um objeto não satisfizerem esse filtro não será mais processado.</span><span class="sxs-lookup"><span data-stu-id="3da93-133">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="3da93-134">É importante entender é que se um objeto usado para atender a esse filtro em um determinado momento, e, em seguida, o objeto ou o filtro foi alterado isso esse filtro não está mais satisfeito, tais objeto *não sejam provisionados desprovisionamento*.</span><span class="sxs-lookup"><span data-stu-id="3da93-134">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="3da93-135">Um objeto é considerado no escopo \*se qualquer um dos grupos na coleção é avaliada para `true` \*.</span><span class="sxs-lookup"><span data-stu-id="3da93-135">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3da93-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3da93-136">JSON representation</span></span>

<span data-ttu-id="3da93-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3da93-137">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
