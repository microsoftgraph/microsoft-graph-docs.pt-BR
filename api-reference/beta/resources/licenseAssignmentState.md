---
title: tipo de recurso de licenseAssignmentState
description: 'A propriedade **licenseAssignmentStates** da entidade do usuário é uma coleção de **licenseAssignmentState**. Ela fornece detalhes sobre as atribuições de licença a um usuário. Os detalhes inclui informações como:  '
ms.openlocfilehash: 4e7101acc756a845913a081368b79242834ef3bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038891"
---
# <a name="licenseassignmentstate-resource-type"></a><span data-ttu-id="37b7b-105">tipo de recurso de licenseAssignmentState</span><span class="sxs-lookup"><span data-stu-id="37b7b-105">licenseAssignmentState resource type</span></span>

> <span data-ttu-id="37b7b-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="37b7b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37b7b-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37b7b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37b7b-108">A propriedade **licenseAssignmentStates** da entidade do [usuário](user.md) é uma coleção de **licenseAssignmentState**.</span><span class="sxs-lookup"><span data-stu-id="37b7b-108">The **licenseAssignmentStates** property of the [user](user.md) entity is a collection of **licenseAssignmentState**.</span></span> <span data-ttu-id="37b7b-109">Ela fornece detalhes sobre as atribuições de licença a um usuário.</span><span class="sxs-lookup"><span data-stu-id="37b7b-109">It provides details about license assignments to a user.</span></span> <span data-ttu-id="37b7b-110">Os detalhes inclui informações como:</span><span class="sxs-lookup"><span data-stu-id="37b7b-110">The details includes information like:</span></span>  

 - <span data-ttu-id="37b7b-111">Quais planos estão desabilitados para um usuário</span><span class="sxs-lookup"><span data-stu-id="37b7b-111">What plans are disabled for a user</span></span>
 - <span data-ttu-id="37b7b-112">Se a licença foi atribuída ao usuário diretamente ou herdada de um grupo</span><span class="sxs-lookup"><span data-stu-id="37b7b-112">Whether the license was assigned to the user directly or inherited from a group</span></span>
 - <span data-ttu-id="37b7b-113">Estado atual da atribuição</span><span class="sxs-lookup"><span data-stu-id="37b7b-113">Current state of the assignment</span></span>
 - <span data-ttu-id="37b7b-114">Se o estado de atribuição for erro, o que é detalhes do erro da falha?</span><span class="sxs-lookup"><span data-stu-id="37b7b-114">If the assignment state is Error, what is the error detail for the failure?</span></span> 


## <a name="properties"></a><span data-ttu-id="37b7b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37b7b-115">Properties</span></span>
| <span data-ttu-id="37b7b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37b7b-116">Property</span></span>     | <span data-ttu-id="37b7b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="37b7b-117">Type</span></span>   |<span data-ttu-id="37b7b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b7b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37b7b-119">assignedByGroup</span><span class="sxs-lookup"><span data-stu-id="37b7b-119">assignedByGroup</span></span>|<span data-ttu-id="37b7b-120">string</span><span class="sxs-lookup"><span data-stu-id="37b7b-120">string</span></span>|<span data-ttu-id="37b7b-121">A identificação do grupo que atribui essa licença.</span><span class="sxs-lookup"><span data-stu-id="37b7b-121">The id of the group that assigns this license.</span></span> <span data-ttu-id="37b7b-122">Se a atribuição for uma licença atribuído diretamente, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="37b7b-122">If the assignment is a direct-assigned license, this field will be Null.</span></span> <span data-ttu-id="37b7b-123">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="37b7b-123">Read-Only.</span></span>|
|<span data-ttu-id="37b7b-124">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="37b7b-124">disabledPlans</span></span>|<span data-ttu-id="37b7b-125">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="37b7b-125">Collection(String)</span></span>|<span data-ttu-id="37b7b-126">Os planos de serviço que serão desabilitados nessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="37b7b-126">The service plans that are disabled in this assignment.</span></span> <span data-ttu-id="37b7b-127">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="37b7b-127">Read-Only.</span></span>|
|<span data-ttu-id="37b7b-128">erro</span><span class="sxs-lookup"><span data-stu-id="37b7b-128">error</span></span>|<span data-ttu-id="37b7b-129">String</span><span class="sxs-lookup"><span data-stu-id="37b7b-129">String</span></span>|<span data-ttu-id="37b7b-130">Erro de falha de atribuição de licença.</span><span class="sxs-lookup"><span data-stu-id="37b7b-130">License assignment failure error.</span></span> <span data-ttu-id="37b7b-131">Se a licença foi distribuída com êxito, esse campo será Null.</span><span class="sxs-lookup"><span data-stu-id="37b7b-131">If the license is assigned successfully, this field will be Null.</span></span> <span data-ttu-id="37b7b-132">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="37b7b-132">Read-Only.</span></span> <span data-ttu-id="37b7b-133">Valores possíveis: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, e `Others`.</span><span class="sxs-lookup"><span data-stu-id="37b7b-133">Possible values: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, and `Others`.</span></span> <span data-ttu-id="37b7b-134">Para obter mais informações sobre como identificar e resolver a atribuição de licença erros consulte [aqui](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span><span class="sxs-lookup"><span data-stu-id="37b7b-134">For more information on how to identify and resolve license assignment errors see [here](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).</span></span>|
|<span data-ttu-id="37b7b-135">skuId</span><span class="sxs-lookup"><span data-stu-id="37b7b-135">skuId</span></span>|<span data-ttu-id="37b7b-136">String</span><span class="sxs-lookup"><span data-stu-id="37b7b-136">String</span></span>|<span data-ttu-id="37b7b-137">O identificador exclusivo da SKU.</span><span class="sxs-lookup"><span data-stu-id="37b7b-137">The unique identifier for the SKU.</span></span> <span data-ttu-id="37b7b-138">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="37b7b-138">Read-Only.</span></span>|
|<span data-ttu-id="37b7b-139">state</span><span class="sxs-lookup"><span data-stu-id="37b7b-139">state</span></span>|<span data-ttu-id="37b7b-140">String</span><span class="sxs-lookup"><span data-stu-id="37b7b-140">String</span></span>|<span data-ttu-id="37b7b-141">Indica o estado atual dessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="37b7b-141">Indicate the current state of this assignment.</span></span> <span data-ttu-id="37b7b-142">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="37b7b-142">Read-Only.</span></span> <span data-ttu-id="37b7b-143">Valores possíveis: ativo, ActiveWithError, desabilitado e erro.</span><span class="sxs-lookup"><span data-stu-id="37b7b-143">Possible values: Active, ActiveWithError, Disabled and Error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37b7b-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37b7b-144">JSON representation</span></span>

<span data-ttu-id="37b7b-145">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="37b7b-145">Here is a JSON representation of the resource</span></span>

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```