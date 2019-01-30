---
title: tipo de recurso de licenseAssignmentState
description: 'A propriedade **licenseAssignmentStates** da entidade do usuário é uma coleção de **licenseAssignmentState**. Ela fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes inclui informações como:  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641677"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="b638f-105">tipo de recurso de licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="b638f-105">licenseAssignmentState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b638f-106">A propriedade **licenseAssignmentStates** da entidade do [usuário](user.md) é uma coleção de **licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="b638f-106">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="b638f-107">Ela fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="b638f-107">It provides details about license assignments to a user.</span></span> <span data-ttu-id="b638f-108">Os detalhes inclui informações como:</span><span class="sxs-lookup"><span data-stu-id="b638f-108">The details includes information like:</span></span>  

 - <span data-ttu-id="b638f-109">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="b638f-109">What plans are disabled for a user</span></span>
 - <span data-ttu-id="b638f-110">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="b638f-110">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="b638f-111">Estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="b638f-111">Current state of the assignment</span></span>
 - <span data-ttu-id="b638f-112">Se o estado de atribuição for erro, o que é detalhes do erro da falha?</span><span class="sxs-lookup"><span data-stu-id="b638f-112">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="b638f-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b638f-113">Properties</span></span>
| <span data-ttu-id="b638f-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b638f-114">Property</span></span>     | <span data-ttu-id="b638f-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b638f-115">Type</span></span>   |<span data-ttu-id="b638f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b638f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b638f-117">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="b638f-117">assignedByGroup</span></span>|<span data-ttu-id="b638f-118">string</span><span class="sxs-lookup"><span data-stu-id="b638f-118">string</span></span>|<span data-ttu-id="b638f-119">A identificação do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="b638f-119">The id of the group that assigns this license.</span></span> <span data-ttu-id="b638f-120">Se a atribuição for uma licença atribuído diretamente, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="b638f-120">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="b638f-121">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b638f-121">Read-Only.</span></span>|
|<span data-ttu-id="b638f-122">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="b638f-122">disabledPlans</span></span>|<span data-ttu-id="b638f-123">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="b638f-123">Collection(String)</span></span>|<span data-ttu-id="b638f-124">Os planos de serviço que serão desabilitados nessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="b638f-124">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="b638f-125">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b638f-125">Read-Only.</span></span>|
|<span data-ttu-id="b638f-126">erro</span><span class="sxs-lookup"><span data-stu-id="b638f-126">error</span></span>|<span data-ttu-id="b638f-127">String</span><span class="sxs-lookup"><span data-stu-id="b638f-127">String</span></span>|<span data-ttu-id="b638f-128">Erro de falha de atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="b638f-128">License assignment failure error.</span></span> <span data-ttu-id="b638f-129">Se a licença foi distribuída com êxito, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="b638f-129">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="b638f-130">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b638f-130">Read-Only.</span></span> <span data-ttu-id="b638f-131">Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, e `Others`.</span><span class="sxs-lookup"><span data-stu-id="b638f-131">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="b638f-132">Para obter mais informações sobre como identificar e resolver a atribuição de licença erros consulte [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="b638f-132">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="b638f-133">skuId</span><span class="sxs-lookup"><span data-stu-id="b638f-133">skuId</span></span>|<span data-ttu-id="b638f-134">String</span><span class="sxs-lookup"><span data-stu-id="b638f-134">String</span></span>|<span data-ttu-id="b638f-135">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="b638f-135">The unique identifier for the SKU.</span></span> <span data-ttu-id="b638f-136">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b638f-136">Read-Only.</span></span>|
|<span data-ttu-id="b638f-137">state</span><span class="sxs-lookup"><span data-stu-id="b638f-137">state</span></span>|<span data-ttu-id="b638f-138">String</span><span class="sxs-lookup"><span data-stu-id="b638f-138">String</span></span>|<span data-ttu-id="b638f-139">Indica o estado atual dessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="b638f-139">Indicate the current state of this assignment.</span></span> <span data-ttu-id="b638f-140">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b638f-140">Read-Only.</span></span> <span data-ttu-id="b638f-141">Valores possíveis: ativo, ActiveWithError, desabilitado e erro.</span><span class="sxs-lookup"><span data-stu-id="b638f-141">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b638f-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b638f-142">JSON representation</span></span>

<span data-ttu-id="b638f-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b638f-143">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
