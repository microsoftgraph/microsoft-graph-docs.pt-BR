---
title: tipo de recurso de licenseAssignmentState
description: A propriedade **licenseAssignmentStates** da entidade do usuário é uma coleção de objetos **licenseAssignmentState** . Ela fornece detalhes sobre as atribuições de licença a um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649365"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="9cbf4-104">tipo de recurso de licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="9cbf4-104">licenseAssignmentState resource type</span></span>


<span data-ttu-id="9cbf4-105">A propriedade **licenseAssignmentStates** da entidade do [usuário](user.md) é uma coleção de objetos **licenseAssignmentState** .</span><span class="sxs-lookup"><span data-stu-id="9cbf4-105">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState** objects.</span></span> <span data-ttu-id="9cbf4-106">Ela fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-106">It provides details about license assignments to a user.</span></span> <span data-ttu-id="9cbf4-107">Os detalhes incluem informações como:</span><span class="sxs-lookup"><span data-stu-id="9cbf4-107">The details include information such as:</span></span>  

 - <span data-ttu-id="9cbf4-108">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="9cbf4-108">What plans are disabled for a user</span></span>
 - <span data-ttu-id="9cbf4-109">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="9cbf4-109">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="9cbf4-110">O estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="9cbf4-110">The current state of the assignment</span></span>
 - <span data-ttu-id="9cbf4-111">Detalhes do erro se o estado de atribuição for erro</span><span class="sxs-lookup"><span data-stu-id="9cbf4-111">Error details if the assignment state is Error</span></span> 


## <a name="properties"></a><span data-ttu-id="9cbf4-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cbf4-112">Properties</span></span>
| <span data-ttu-id="9cbf4-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cbf4-113">Property</span></span>     | <span data-ttu-id="9cbf4-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cbf4-114">Type</span></span>   |<span data-ttu-id="9cbf4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cbf4-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9cbf4-116">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="9cbf4-116">assignedByGroup</span></span>|<span data-ttu-id="9cbf4-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9cbf4-117">string</span></span>|<span data-ttu-id="9cbf4-118">A identificação do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-118">The id of the group that assigns this license.</span></span> <span data-ttu-id="9cbf4-119">Se a atribuição for uma licença atribuído diretamente, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-119">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="9cbf4-120">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-120">Read-Only.</span></span>|
|<span data-ttu-id="9cbf4-121">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="9cbf4-121">disabledPlans</span></span>|<span data-ttu-id="9cbf4-122">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="9cbf4-122">Collection(String)</span></span>|<span data-ttu-id="9cbf4-123">Os planos de serviço que serão desabilitados nessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-123">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="9cbf4-124">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-124">Read-Only.</span></span>|
|<span data-ttu-id="9cbf4-125">erro</span><span class="sxs-lookup"><span data-stu-id="9cbf4-125">error</span></span>|<span data-ttu-id="9cbf4-126">String</span><span class="sxs-lookup"><span data-stu-id="9cbf4-126">String</span></span>|<span data-ttu-id="9cbf4-127">Erro de falha de atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-127">License assignment failure error.</span></span> <span data-ttu-id="9cbf4-128">Se a licença foi distribuída com êxito, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-128">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="9cbf4-129">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-129">Read-Only.</span></span> <span data-ttu-id="9cbf4-130">Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, e `Others`.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-130">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="9cbf4-131">Para obter mais informações sobre como identificar e resolver a atribuição de licença erros consulte [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="9cbf4-131">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="9cbf4-132">skuId</span><span class="sxs-lookup"><span data-stu-id="9cbf4-132">skuId</span></span>|<span data-ttu-id="9cbf4-133">String</span><span class="sxs-lookup"><span data-stu-id="9cbf4-133">String</span></span>|<span data-ttu-id="9cbf4-134">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-134">The unique identifier for the SKU.</span></span> <span data-ttu-id="9cbf4-135">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-135">Read-Only.</span></span>|
|<span data-ttu-id="9cbf4-136">state</span><span class="sxs-lookup"><span data-stu-id="9cbf4-136">state</span></span>|<span data-ttu-id="9cbf4-137">String</span><span class="sxs-lookup"><span data-stu-id="9cbf4-137">String</span></span>|<span data-ttu-id="9cbf4-138">Indica o estado atual dessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-138">Indicate the current state of this assignment.</span></span> <span data-ttu-id="9cbf4-139">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-139">Read-Only.</span></span> <span data-ttu-id="9cbf4-140">Valores possíveis: ativo, ActiveWithError, desabilitado e erro.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-140">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9cbf4-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cbf4-141">JSON representation</span></span>

<span data-ttu-id="9cbf4-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cbf4-142">The following is a JSON representation of the resource.</span></span>

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
