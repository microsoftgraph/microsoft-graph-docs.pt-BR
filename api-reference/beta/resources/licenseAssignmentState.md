---
title: tipo de recurso licenseAssignmentState
description: 'A propriedade **licenseAssignmentStates** da entidade User é uma coleção de **licenseAssignmentState**. Ele fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes incluem informações como:  '
localization_priority: Normal
ms.openlocfilehash: e720070c4c97c58fd3c99e49656d7ca33f5fb9d4
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778422"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="51807-105">tipo de recurso licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="51807-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51807-106">A propriedade **licenseAssignmentStates** da entidade [User](user.md) é uma coleção de **licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="51807-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="51807-107">Ele fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="51807-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="51807-108">Os detalhes incluem informações como:</span><span class="sxs-lookup"><span data-stu-id="51807-108">The details includes information like:</span></span>  

- <span data-ttu-id="51807-109">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="51807-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="51807-110">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="51807-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="51807-111">Estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="51807-111">Current state of the assignment</span></span>
- <span data-ttu-id="51807-112">Se o estado da atribuição for erro, qual é o detalhe do erro para a falha?</span><span class="sxs-lookup"><span data-stu-id="51807-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="51807-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51807-113">Properties</span></span>
| <span data-ttu-id="51807-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51807-114">Property</span></span>     | <span data-ttu-id="51807-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="51807-115">Type</span></span>   |<span data-ttu-id="51807-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="51807-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51807-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="51807-117">assignedByGroup</span></span>|<span data-ttu-id="51807-118">string</span><span class="sxs-lookup"><span data-stu-id="51807-118">string</span></span>|<span data-ttu-id="51807-119">A ID do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="51807-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="51807-120">Se a atribuição for uma licença atribuída diretamente, esse campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="51807-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="51807-121">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="51807-121">Read-Only.</span></span>|
|<span data-ttu-id="51807-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="51807-122">disabledPlans</span></span>|<span data-ttu-id="51807-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="51807-123">Collection(String)</span></span>|<span data-ttu-id="51807-124">Os planos de serviço que estão desabilitados nesta atribuição.</span><span class="sxs-lookup"><span data-stu-id="51807-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="51807-125">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="51807-125">Read-Only.</span></span>|
|<span data-ttu-id="51807-126">erro</span><span class="sxs-lookup"><span data-stu-id="51807-126">error</span></span>|<span data-ttu-id="51807-127">String</span><span class="sxs-lookup"><span data-stu-id="51807-127">String</span></span>|<span data-ttu-id="51807-128">Erro de falha na atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="51807-128">License assignment failure error.</span></span> <span data-ttu-id="51807-129">Se a licença for atribuída com êxito, este campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="51807-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="51807-130">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="51807-130">Read-Only.</span></span> <span data-ttu-id="51807-131">Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`,, e `Others`.</span><span class="sxs-lookup"><span data-stu-id="51807-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="51807-132">Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, confira [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="51807-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="51807-133">skuId</span><span class="sxs-lookup"><span data-stu-id="51807-133">skuId</span></span>|<span data-ttu-id="51807-134">String</span><span class="sxs-lookup"><span data-stu-id="51807-134">String</span></span>|<span data-ttu-id="51807-135">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="51807-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="51807-136">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="51807-136">Read-Only.</span></span>|
|<span data-ttu-id="51807-137">state</span><span class="sxs-lookup"><span data-stu-id="51807-137">state</span></span>|<span data-ttu-id="51807-138">String</span><span class="sxs-lookup"><span data-stu-id="51807-138">String</span></span>|<span data-ttu-id="51807-139">Indica o estado atual desta atribuição.</span><span class="sxs-lookup"><span data-stu-id="51807-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="51807-140">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="51807-140">Read-Only.</span></span> <span data-ttu-id="51807-141">Valores possíveis: Active, ActiveWithError, Disabled e Error.</span><span class="sxs-lookup"><span data-stu-id="51807-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51807-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51807-142">JSON representation</span></span>

<span data-ttu-id="51807-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="51807-143">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
