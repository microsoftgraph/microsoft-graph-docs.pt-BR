---
title: Tipo de recurso licenseAssignmentState
description: 'A **propriedade licenseAssignmentStates** da entidade do usuário é uma coleção **de licenseAssignmentState**. Ele fornece detalhes sobre atribuições de licença para um usuário. Os detalhes incluem informações como:  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jpettere
ms.openlocfilehash: 6362737397d8f5b5c1643557bc7c834392b520ef
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720526"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="cf2ad-105">Tipo de recurso licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="cf2ad-105">licenseAssignmentState resource type</span></span>

<span data-ttu-id="cf2ad-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf2ad-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf2ad-107">A **propriedade licenseAssignmentStates** da entidade [do](user.md) usuário é uma coleção **de licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-107">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="cf2ad-108">Ele fornece detalhes sobre atribuições de licença para um usuário.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-108">It provides details about license assignments to a user.</span></span> <span data-ttu-id="cf2ad-109">Os detalhes incluem informações como:</span><span class="sxs-lookup"><span data-stu-id="cf2ad-109">The details includes information like:</span></span>

- <span data-ttu-id="cf2ad-110">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="cf2ad-110">What plans are disabled for a user</span></span>
- <span data-ttu-id="cf2ad-111">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="cf2ad-111">Whether the license was assigned to the user directly or inherited from a group</span></span>
- <span data-ttu-id="cf2ad-112">Estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="cf2ad-112">Current state of the assignment</span></span>
- <span data-ttu-id="cf2ad-113">Se o estado da atribuição for Error, qual é o detalhe de erro da falha?</span><span class="sxs-lookup"><span data-stu-id="cf2ad-113">If the assignment state is Error, what is the error detail for the failure?</span></span>


## <a name="properties"></a><span data-ttu-id="cf2ad-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf2ad-114">Properties</span></span>
| <span data-ttu-id="cf2ad-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf2ad-115">Property</span></span>     | <span data-ttu-id="cf2ad-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf2ad-116">Type</span></span>   |<span data-ttu-id="cf2ad-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf2ad-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf2ad-118">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="cf2ad-118">assignedByGroup</span></span>|<span data-ttu-id="cf2ad-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf2ad-119">string</span></span>|<span data-ttu-id="cf2ad-120">A id do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-120">The id of the group that assigns this license.</span></span> <span data-ttu-id="cf2ad-121">Se a atribuição for uma licença atribuída diretamente, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-121">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="cf2ad-122">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-122">Read-Only.</span></span>|
|<span data-ttu-id="cf2ad-123">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="cf2ad-123">disabledPlans</span></span>|<span data-ttu-id="cf2ad-124">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="cf2ad-124">Collection(String)</span></span>|<span data-ttu-id="cf2ad-125">Os planos de serviço que estão desabilitados nesta atribuição.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-125">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="cf2ad-126">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-126">Read-Only.</span></span>|
|<span data-ttu-id="cf2ad-127">erro</span><span class="sxs-lookup"><span data-stu-id="cf2ad-127">error</span></span>|<span data-ttu-id="cf2ad-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf2ad-128">String</span></span>|<span data-ttu-id="cf2ad-129">Erro de falha de atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-129">License assignment failure error.</span></span> <span data-ttu-id="cf2ad-130">Se a licença for atribuída com êxito, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-130">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="cf2ad-131">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-131">Read-Only.</span></span> <span data-ttu-id="cf2ad-132">Valores possíveis: `CountViolation` , , , , e `MutuallyExclusiveViolation` `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation` `Others` .</span><span class="sxs-lookup"><span data-stu-id="cf2ad-132">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="cf2ad-133">Para obter mais informações sobre como identificar e resolver erros de atribuição de licença, [consulte aqui](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="cf2ad-133">For more information on how to identify and resolve license assignment errors see [here](/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="cf2ad-134">skuId</span><span class="sxs-lookup"><span data-stu-id="cf2ad-134">skuId</span></span>|<span data-ttu-id="cf2ad-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf2ad-135">String</span></span>|<span data-ttu-id="cf2ad-136">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-136">The unique identifier for the SKU.</span></span> <span data-ttu-id="cf2ad-137">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-137">Read-Only.</span></span>|
|<span data-ttu-id="cf2ad-138">estado</span><span class="sxs-lookup"><span data-stu-id="cf2ad-138">state</span></span>|<span data-ttu-id="cf2ad-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf2ad-139">String</span></span>|<span data-ttu-id="cf2ad-140">Indique o estado atual dessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-140">Indicate the current state of this assignment.</span></span> <span data-ttu-id="cf2ad-141">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-141">Read-Only.</span></span> <span data-ttu-id="cf2ad-142">Valores possíveis: Active, ActiveWithError, Disabled e Error.</span><span class="sxs-lookup"><span data-stu-id="cf2ad-142">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf2ad-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf2ad-143">JSON representation</span></span>

<span data-ttu-id="cf2ad-144">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cf2ad-144">Here is a JSON representation of the resource</span></span>

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