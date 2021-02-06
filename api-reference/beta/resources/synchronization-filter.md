---
title: tipo de recurso filter
description: Determina quais objetos devem ser provisionados para o aplicativo.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8c461dffab9af810d20f6b866134ecc5d4238eb1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133928"
---
# <a name="filter-resource-type"></a><span data-ttu-id="829b9-103">tipo de recurso filter</span><span class="sxs-lookup"><span data-stu-id="829b9-103">filter resource type</span></span>

<span data-ttu-id="829b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="829b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="829b9-105">Determina quais objetos devem ser provisionados para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="829b9-105">Determines which objects should be provisioned to the application.</span></span> <span data-ttu-id="829b9-106">Por exemplo, talvez você queira provisionar apenas usuários localizados nos EUA.</span><span class="sxs-lookup"><span data-stu-id="829b9-106">For example, you might want to only provision users that are located in the US.</span></span> <span data-ttu-id="829b9-107">Quando um filtro de scoping estiver presente, os objetos que não satisfazem o filtro serão ignorados durante a sincronização.</span><span class="sxs-lookup"><span data-stu-id="829b9-107">When a scoping filter is present, objects that do not satisfy the filter will be skipped during synchronization.</span></span>

<span data-ttu-id="829b9-108">O filtro faz parte do [mapeamento de objetos.](synchronization-objectmapping.md)</span><span class="sxs-lookup"><span data-stu-id="829b9-108">Filter is part of [object mapping](synchronization-objectmapping.md).</span></span> <span data-ttu-id="829b9-109">Ele consiste em vários conjuntos de grupos de filtros, e cada grupo de filtros contém uma ou mais cláusulas.</span><span class="sxs-lookup"><span data-stu-id="829b9-109">It consists of several sets of filter groups, and each filter group holds one or more clauses.</span></span> <span data-ttu-id="829b9-110">Um objeto é considerado no escopo do grupo (o grupo é avaliado para ) somente se todas as cláusulas do grupo `true` são avaliadas para `true` .</span><span class="sxs-lookup"><span data-stu-id="829b9-110">An object is considered in scope for the group (the group is evaluated to `true`) only if all the clauses of the group are evaluated to `true`.</span></span>

<span data-ttu-id="829b9-111">Um objeto é considerado no escopo do conjunto de grupos (o conjunto de grupos é avaliado como ) se qualquer um dos grupos no conjunto `true` for avaliado como `true` .</span><span class="sxs-lookup"><span data-stu-id="829b9-111">An object is considered in scope for the group set (group set is evaluated to `true`) if any of the groups in the set is evaluated to `true`.</span></span>

<span data-ttu-id="829b9-112">Para obter mais informações, consulte [Provisionamento de aplicativo baseado em atributo com filtros de scoping](/azure/active-directory/active-directory-saas-scoping-filters)</span><span class="sxs-lookup"><span data-stu-id="829b9-112">For more information, see [Attribute-based application provisioning with scoping filters](/azure/active-directory/active-directory-saas-scoping-filters)</span></span>

## <a name="properties"></a><span data-ttu-id="829b9-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="829b9-113">Properties</span></span>
| <span data-ttu-id="829b9-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="829b9-114">Property</span></span>     | <span data-ttu-id="829b9-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="829b9-115">Type</span></span>   |<span data-ttu-id="829b9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="829b9-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="829b9-117">categoryFilterGroups</span><span class="sxs-lookup"><span data-stu-id="829b9-117">categoryFilterGroups</span></span>|<span data-ttu-id="829b9-118">[coleção filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="829b9-118">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="829b9-119">`*Experimental*` Conjunto de grupos de filtros usado para decidir se determinado objeto pertence e deve ser processado como parte desse mapeamento de objeto.</span><span class="sxs-lookup"><span data-stu-id="829b9-119">`*Experimental*` Filter group set used to decide whether given object belongs and should be processed as part of this object mapping.</span></span> <span data-ttu-id="829b9-120">Um objeto será considerado no *escopo se QUALQUER um `true` dos grupos na coleção for avaliado como*.</span><span class="sxs-lookup"><span data-stu-id="829b9-120">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="829b9-121">grupos</span><span class="sxs-lookup"><span data-stu-id="829b9-121">groups</span></span>|<span data-ttu-id="829b9-122">[coleção filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="829b9-122">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="829b9-123">Conjunto de grupos de filtros usado para decidir se determinado objeto está no escopo do provisionamento.</span><span class="sxs-lookup"><span data-stu-id="829b9-123">Filter group set used to decide whether given object is in scope for provisioning.</span></span> <span data-ttu-id="829b9-124">**Este é o filtro que deve ser usado na maioria dos casos.**</span><span class="sxs-lookup"><span data-stu-id="829b9-124">**This is the filter which should be used in most cases**.</span></span> <span data-ttu-id="829b9-125">Se um objeto usado para satisfazer esse filtro em um dado momento e, em seguida, o objeto ou o filtro foi alterado para que o filtro não seja mais satisfeito, esse objeto \*será des-provisionado".</span><span class="sxs-lookup"><span data-stu-id="829b9-125">If an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is not satisfied any longer, such object \*will get de-provisioned".</span></span> <span data-ttu-id="829b9-126">Um objeto será considerado no *escopo se QUALQUER um `true` dos grupos na coleção for avaliado como*.</span><span class="sxs-lookup"><span data-stu-id="829b9-126">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span>|
|<span data-ttu-id="829b9-127">inputFilterGroups</span><span class="sxs-lookup"><span data-stu-id="829b9-127">inputFilterGroups</span></span>|<span data-ttu-id="829b9-128">[coleção filterGroup](synchronization-filtergroup.md)</span><span class="sxs-lookup"><span data-stu-id="829b9-128">[filterGroup](synchronization-filtergroup.md) collection</span></span>|<span data-ttu-id="829b9-129">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span><span class="sxs-lookup"><span data-stu-id="829b9-129">`*Experimental*` Filter group set used to filter out objects at the early stage of reading them from the directory.</span></span> <span data-ttu-id="829b9-130">Se um objeto não satisfaça esse filtro, ele não será processado ainda mais.</span><span class="sxs-lookup"><span data-stu-id="829b9-130">If an object doesn't satisfy this filter it will not be processed further.</span></span> <span data-ttu-id="829b9-131">É importante entender que, se um objeto usado para satisfazer esse filtro em um determinado momento e, em seguida, o objeto ou o filtro foi alterado para que o filtro não seja mais satisfeito, esse objeto NÃO será *des* provisionado.</span><span class="sxs-lookup"><span data-stu-id="829b9-131">Important to understand is that if an object used to satisfy this filter at a given moment, and then the object or the filter was changed so that filter is no longer satisfied, such object *will NOT get de-provisioned*.</span></span> <span data-ttu-id="829b9-132">Um objeto será considerado no *escopo se QUALQUER um `true` dos grupos na coleção for avaliado como*.</span><span class="sxs-lookup"><span data-stu-id="829b9-132">An object is considered in scope *if ANY of the groups in the collection is evaluated to `true`*.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="829b9-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="829b9-133">JSON representation</span></span>

<span data-ttu-id="829b9-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="829b9-134">Here is a JSON representation of the resource.</span></span>

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


