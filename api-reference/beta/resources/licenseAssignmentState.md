---
title: tipo de recurso licenseAssignmentState
description: 'A propriedade **licenseAssignmentStates** da entidade User é uma coleção de **licenseAssignmentState**. Ele fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes incluem informações como:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: f0032c9b32ba068b0ccaf7c2e4cafb8a775184da
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401782"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="0f77f-105">tipo de recurso licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="0f77f-105">licenseAssignmentState resource type</span></span>

<span data-ttu-id="0f77f-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f77f-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f77f-107">A propriedade **licenseAssignmentStates** da entidade [User](user.md) é uma coleção de **licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="0f77f-107">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="0f77f-108">Ele fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="0f77f-108">It provides details about license assignments to a user.</span></span> <span data-ttu-id="0f77f-109">Os detalhes incluem informações como:</span><span class="sxs-lookup"><span data-stu-id="0f77f-109">The details includes information like:</span></span>

- <span data-ttu-id="0f77f-110">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="0f77f-110">What plans are disabled for a user</span></span>
- <span data-ttu-id="0f77f-111">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="0f77f-111">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="0f77f-112">Estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="0f77f-112">Current state of the assignment</span></span>
- <span data-ttu-id="0f77f-113">Se o estado da atribuição for erro, qual é o detalhe do erro para a falha?</span><span class="sxs-lookup"><span data-stu-id="0f77f-113">If the assignment state is Error, what is the error detail for the failure?</span></span>


## <a name="properties"></a><span data-ttu-id="0f77f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f77f-114">Properties</span></span>
| <span data-ttu-id="0f77f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f77f-115">Property</span></span>     | <span data-ttu-id="0f77f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f77f-116">Type</span></span>   |<span data-ttu-id="0f77f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f77f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f77f-118">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="0f77f-118">assignedByGroup</span></span>|<span data-ttu-id="0f77f-119">string</span><span class="sxs-lookup"><span data-stu-id="0f77f-119">string</span></span>|<span data-ttu-id="0f77f-120">A ID do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="0f77f-120">The id of the group that assigns this license.</span></span> <span data-ttu-id="0f77f-121">Se a atribuição for uma licença atribuída diretamente, esse campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="0f77f-121">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="0f77f-122">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0f77f-122">Read-Only.</span></span>|
|<span data-ttu-id="0f77f-123">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="0f77f-123">disabledPlans</span></span>|<span data-ttu-id="0f77f-124">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="0f77f-124">Collection(String)</span></span>|<span data-ttu-id="0f77f-125">Os planos de serviço que estão desabilitados nesta atribuição.</span><span class="sxs-lookup"><span data-stu-id="0f77f-125">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="0f77f-126">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0f77f-126">Read-Only.</span></span>|
|<span data-ttu-id="0f77f-127">erro</span><span class="sxs-lookup"><span data-stu-id="0f77f-127">error</span></span>|<span data-ttu-id="0f77f-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f77f-128">String</span></span>|<span data-ttu-id="0f77f-129">Erro de falha na atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="0f77f-129">License assignment failure error.</span></span> <span data-ttu-id="0f77f-130">Se a licença for atribuída com êxito, este campo será nulo.</span><span class="sxs-lookup"><span data-stu-id="0f77f-130">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="0f77f-131">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0f77f-131">Read-Only.</span></span> <span data-ttu-id="0f77f-132">Valores possíveis: `CountViolation` , `MutuallyExclusiveViolation` ,,, `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` e `Others` .</span><span class="sxs-lookup"><span data-stu-id="0f77f-132">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="0f77f-133">Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, confira [aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="0f77f-133">For more information on how to identify and resolve license assignment errors see [here](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="0f77f-134">skuId</span><span class="sxs-lookup"><span data-stu-id="0f77f-134">skuId</span></span>|<span data-ttu-id="0f77f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f77f-135">String</span></span>|<span data-ttu-id="0f77f-136">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="0f77f-136">The unique identifier for the SKU.</span></span> <span data-ttu-id="0f77f-137">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0f77f-137">Read-Only.</span></span>|
|<span data-ttu-id="0f77f-138">estado</span><span class="sxs-lookup"><span data-stu-id="0f77f-138">state</span></span>|<span data-ttu-id="0f77f-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f77f-139">String</span></span>|<span data-ttu-id="0f77f-140">Indica o estado atual desta atribuição.</span><span class="sxs-lookup"><span data-stu-id="0f77f-140">Indicate the current state of this assignment.</span></span> <span data-ttu-id="0f77f-141">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0f77f-141">Read-Only.</span></span> <span data-ttu-id="0f77f-142">Valores possíveis: Active, ActiveWithError, Disabled e Error.</span><span class="sxs-lookup"><span data-stu-id="0f77f-142">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f77f-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f77f-143">JSON representation</span></span>

<span data-ttu-id="0f77f-144">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0f77f-144">Here is a JSON representation of the resource</span></span>

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