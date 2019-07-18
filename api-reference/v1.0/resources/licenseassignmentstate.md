---
title: tipo de recurso licenseAssignmentState
description: A propriedade **licenseAssignmentStates** da entidade User é uma coleção de objetos **licenseAssignmentState** . Ele fornece detalhes sobre as atribuições de licença a um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 358c54ae2562479734cc496b1fe9ab8eb34812fa
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778688"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="c40d1-104">tipo de recurso licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="c40d1-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="c40d1-105">A propriedade **licenseAssignmentStates** da entidade [User](user.md) é uma coleção de objetos **licenseAssignmentState** .</span><span class="sxs-lookup"><span data-stu-id="c40d1-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="c40d1-106">Ele fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c40d1-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="c40d1-107">Os detalhes incluem informações como:</span><span class="sxs-lookup"><span data-stu-id="c40d1-107">The details include information such as:</span></span>  

- <span data-ttu-id="c40d1-108">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="c40d1-108">What plans are disabled for a user</span></span>
- <span data-ttu-id="c40d1-109">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="c40d1-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="c40d1-110">O estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="c40d1-110">The current state of the assignment</span></span>
- <span data-ttu-id="c40d1-111">Detalhes do erro se o estado da atribuição for erro</span><span class="sxs-lookup"><span data-stu-id="c40d1-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="c40d1-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c40d1-112">Properties</span></span>
| <span data-ttu-id="c40d1-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c40d1-113">Property</span></span>     | <span data-ttu-id="c40d1-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c40d1-114">Type</span></span>   |<span data-ttu-id="c40d1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c40d1-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c40d1-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="c40d1-116">assignedByGroup</span></span>|<span data-ttu-id="c40d1-117">string</span><span class="sxs-lookup"><span data-stu-id="c40d1-117">string</span></span>|<span data-ttu-id="c40d1-118">A ID do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="c40d1-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="c40d1-119">Se a atribuição for uma licença atribuída diretamente, esse campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="c40d1-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="c40d1-120">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c40d1-120">Read-Only.</span></span>|
|<span data-ttu-id="c40d1-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="c40d1-121">disabledPlans</span></span>|<span data-ttu-id="c40d1-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="c40d1-122">Collection(String)</span></span>|<span data-ttu-id="c40d1-123">Os planos de serviço que estão desabilitados nesta atribuição.</span><span class="sxs-lookup"><span data-stu-id="c40d1-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="c40d1-124">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c40d1-124">Read-Only.</span></span>|
|<span data-ttu-id="c40d1-125">erro</span><span class="sxs-lookup"><span data-stu-id="c40d1-125">error</span></span>|<span data-ttu-id="c40d1-126">String</span><span class="sxs-lookup"><span data-stu-id="c40d1-126">String</span></span>|<span data-ttu-id="c40d1-127">Erro de falha na atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="c40d1-127">License assignment failure error.</span></span> <span data-ttu-id="c40d1-128">Se a licença for atribuída com êxito, este campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="c40d1-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="c40d1-129">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c40d1-129">Read-Only.</span></span> <span data-ttu-id="c40d1-130">Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`,, e `Others`.</span><span class="sxs-lookup"><span data-stu-id="c40d1-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="c40d1-131">Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, confira [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="c40d1-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="c40d1-132">skuId</span><span class="sxs-lookup"><span data-stu-id="c40d1-132">skuId</span></span>|<span data-ttu-id="c40d1-133">String</span><span class="sxs-lookup"><span data-stu-id="c40d1-133">String</span></span>|<span data-ttu-id="c40d1-134">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="c40d1-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="c40d1-135">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c40d1-135">Read-Only.</span></span>|
|<span data-ttu-id="c40d1-136">state</span><span class="sxs-lookup"><span data-stu-id="c40d1-136">state</span></span>|<span data-ttu-id="c40d1-137">String</span><span class="sxs-lookup"><span data-stu-id="c40d1-137">String</span></span>|<span data-ttu-id="c40d1-138">Indica o estado atual desta atribuição.</span><span class="sxs-lookup"><span data-stu-id="c40d1-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="c40d1-139">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c40d1-139">Read-Only.</span></span> <span data-ttu-id="c40d1-140">Valores possíveis: Active, ActiveWithError, Disabled e Error.</span><span class="sxs-lookup"><span data-stu-id="c40d1-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c40d1-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c40d1-141">JSON representation</span></span>

<span data-ttu-id="c40d1-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c40d1-142">The following is a JSON representation of the resource.</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
