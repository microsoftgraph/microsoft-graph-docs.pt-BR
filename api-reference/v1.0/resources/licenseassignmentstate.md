---
title: tipo de recurso licenseAssignmentState
description: A propriedade **licenseAssignmentStates** da entidade User é uma coleção de objetos **licenseAssignmentState** . Ele fornece detalhes sobre as atribuições de licença a um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: b26ab4be63cbb40929dbea3f40522ee4c6b7ff70
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582181"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="686fa-104">tipo de recurso licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="686fa-104">licenseAssignmentState resource type</span></span>

<span data-ttu-id="686fa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="686fa-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="686fa-106">A propriedade **licenseAssignmentStates** da entidade [User](user.md) é uma coleção de objetos **licenseAssignmentState** .</span><span class="sxs-lookup"><span data-stu-id="686fa-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="686fa-107">Ele fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="686fa-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="686fa-108">Os detalhes incluem informações como:</span><span class="sxs-lookup"><span data-stu-id="686fa-108">The details include information such as:</span></span>  

- <span data-ttu-id="686fa-109">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="686fa-109">What plans are disabled for a user</span></span>
- <span data-ttu-id="686fa-110">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="686fa-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="686fa-111">O estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="686fa-111">The current state of the assignment</span></span>
- <span data-ttu-id="686fa-112">Detalhes do erro se o estado da atribuição for erro</span><span class="sxs-lookup"><span data-stu-id="686fa-112">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="686fa-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="686fa-113">Properties</span></span>
| <span data-ttu-id="686fa-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="686fa-114">Property</span></span>     | <span data-ttu-id="686fa-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="686fa-115">Type</span></span>   |<span data-ttu-id="686fa-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="686fa-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="686fa-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="686fa-117">assignedByGroup</span></span>|<span data-ttu-id="686fa-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686fa-118">string</span></span>|<span data-ttu-id="686fa-119">A ID do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="686fa-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="686fa-120">Se a atribuição for uma licença atribuída diretamente, esse campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="686fa-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="686fa-121">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="686fa-121">Read-Only.</span></span>|
|<span data-ttu-id="686fa-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="686fa-122">disabledPlans</span></span>|<span data-ttu-id="686fa-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="686fa-123">Collection(String)</span></span>|<span data-ttu-id="686fa-124">Os planos de serviço que estão desabilitados nesta atribuição.</span><span class="sxs-lookup"><span data-stu-id="686fa-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="686fa-125">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="686fa-125">Read-Only.</span></span>|
|<span data-ttu-id="686fa-126">erro</span><span class="sxs-lookup"><span data-stu-id="686fa-126">error</span></span>|<span data-ttu-id="686fa-127">String</span><span class="sxs-lookup"><span data-stu-id="686fa-127">String</span></span>|<span data-ttu-id="686fa-128">Erro de falha na atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="686fa-128">License assignment failure error.</span></span> <span data-ttu-id="686fa-129">Se a licença for atribuída com êxito, este campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="686fa-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="686fa-130">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="686fa-130">Read-Only.</span></span> <span data-ttu-id="686fa-131">Valores possíveis: `CountViolation` , `MutuallyExclusiveViolation` ,,, `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` e `Others` .</span><span class="sxs-lookup"><span data-stu-id="686fa-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="686fa-132">Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, confira [aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="686fa-132">For more information on how to identify and resolve license assignment errors see [here](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="686fa-133">skuId</span><span class="sxs-lookup"><span data-stu-id="686fa-133">skuId</span></span>|<span data-ttu-id="686fa-134">String</span><span class="sxs-lookup"><span data-stu-id="686fa-134">String</span></span>|<span data-ttu-id="686fa-135">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="686fa-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="686fa-136">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="686fa-136">Read-Only.</span></span>|
|<span data-ttu-id="686fa-137">state</span><span class="sxs-lookup"><span data-stu-id="686fa-137">state</span></span>|<span data-ttu-id="686fa-138">String</span><span class="sxs-lookup"><span data-stu-id="686fa-138">String</span></span>|<span data-ttu-id="686fa-139">Indica o estado atual desta atribuição.</span><span class="sxs-lookup"><span data-stu-id="686fa-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="686fa-140">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="686fa-140">Read-Only.</span></span> <span data-ttu-id="686fa-141">Valores possíveis: Active, ActiveWithError, Disabled e Error.</span><span class="sxs-lookup"><span data-stu-id="686fa-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="686fa-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="686fa-142">JSON representation</span></span>

<span data-ttu-id="686fa-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="686fa-143">The following is a JSON representation of the resource.</span></span>

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