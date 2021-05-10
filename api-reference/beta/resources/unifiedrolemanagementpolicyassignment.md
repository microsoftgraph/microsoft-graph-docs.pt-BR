---
title: Tipo de recurso unifiedRoleManagementPolicyAssignment
description: Um unifiedRoleManagementPolicyAssignment atribui a política a um escopo específico e à definição de função.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3028655cb1b7acd88764abf64dd609147b399a07
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299109"
---
# <a name="unifiedrolemanagementpolicyassignment-resource-type"></a><span data-ttu-id="fdf1e-103">Tipo de recurso unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fdf1e-103">unifiedRoleManagementPolicyAssignment resource type</span></span>

<span data-ttu-id="fdf1e-104">Um unifiedRoleManagementPolicyAssignment atribui a política a um escopo específico e à definição de função.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-104">A unifiedRoleManagementPolicyAssignment assigns the policy to a specific scope and role definition.</span></span>

## <a name="methods"></a><span data-ttu-id="fdf1e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fdf1e-105">Methods</span></span>
|<span data-ttu-id="fdf1e-106">Método</span><span class="sxs-lookup"><span data-stu-id="fdf1e-106">Method</span></span>|<span data-ttu-id="fdf1e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fdf1e-107">Return type</span></span>|<span data-ttu-id="fdf1e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf1e-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fdf1e-109">Listar unifiedRoleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="fdf1e-109">List unifiedRoleManagementPolicyAssignments</span></span>](../api/unifiedrolemanagementpolicyassignment-list.md)|<span data-ttu-id="fdf1e-110">[Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fdf1e-110">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="fdf1e-111">Obter uma lista dos [objetos unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-111">Get a list of the [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) objects and their properties.</span></span>|
|[<span data-ttu-id="fdf1e-112">Obter unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fdf1e-112">Get unifiedRoleManagementPolicyAssignment</span></span>](../api/unifiedrolemanagementpolicyassignment-get.md)|[<span data-ttu-id="fdf1e-113">unifiedRoleManagementPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="fdf1e-113">unifiedRoleManagementPolicyAssignment</span></span>](../resources/unifiedrolemanagementpolicyassignment.md)|<span data-ttu-id="fdf1e-114">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicyAssignment.](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fdf1e-114">Read the properties and relationships of an [unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fdf1e-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdf1e-115">Properties</span></span>
|<span data-ttu-id="fdf1e-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdf1e-116">Property</span></span>|<span data-ttu-id="fdf1e-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdf1e-117">Type</span></span>|<span data-ttu-id="fdf1e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf1e-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf1e-119">id</span><span class="sxs-lookup"><span data-stu-id="fdf1e-119">id</span></span>|<span data-ttu-id="fdf1e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdf1e-120">String</span></span>|<span data-ttu-id="fdf1e-121">Identificador exclusivo da atribuição de política.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-121">Unique identifier for the policy assignment.</span></span>|
|<span data-ttu-id="fdf1e-122">policyId</span><span class="sxs-lookup"><span data-stu-id="fdf1e-122">policyId</span></span>|<span data-ttu-id="fdf1e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdf1e-123">String</span></span>|<span data-ttu-id="fdf1e-124">A id da política.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-124">The id of the policy.</span></span>|
|<span data-ttu-id="fdf1e-125">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fdf1e-125">roleDefinitionId</span></span>|<span data-ttu-id="fdf1e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdf1e-126">String</span></span>|<span data-ttu-id="fdf1e-127">A id da definição de função em que a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-127">The id of the role definition where the policy applies.</span></span> <span data-ttu-id="fdf1e-128">Se não for especificada, a política se aplicará a todas as funções.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-128">If not specified, the policy applies to all roles.</span></span>|
|<span data-ttu-id="fdf1e-129">scopeId</span><span class="sxs-lookup"><span data-stu-id="fdf1e-129">scopeId</span></span>|<span data-ttu-id="fdf1e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdf1e-130">String</span></span>|<span data-ttu-id="fdf1e-131">A id do escopo em que a política é atribuída.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-131">The id of the scope where the policy is assigned.</span></span> <span data-ttu-id="fdf1e-132">Por exemplo</span><span class="sxs-lookup"><span data-stu-id="fdf1e-132">E.g.</span></span> <span data-ttu-id="fdf1e-133">"/", groupId, etc.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-133">"/", groupId, etc.</span></span>|
|<span data-ttu-id="fdf1e-134">scopeType</span><span class="sxs-lookup"><span data-stu-id="fdf1e-134">scopeType</span></span>|<span data-ttu-id="fdf1e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdf1e-135">String</span></span>|<span data-ttu-id="fdf1e-136">O tipo do escopo em que a política é atribuída.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-136">The type of the scope where the policy is assigned.</span></span> <span data-ttu-id="fdf1e-137">Um de Directory, DirectoryRole, Group.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-137">One of Directory, DirectoryRole, Group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdf1e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="fdf1e-138">Relationships</span></span>
|<span data-ttu-id="fdf1e-139">Relação</span><span class="sxs-lookup"><span data-stu-id="fdf1e-139">Relationship</span></span>|<span data-ttu-id="fdf1e-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdf1e-140">Type</span></span>|<span data-ttu-id="fdf1e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf1e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf1e-142">política</span><span class="sxs-lookup"><span data-stu-id="fdf1e-142">policy</span></span>|[<span data-ttu-id="fdf1e-143">unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="fdf1e-143">unifiedRoleManagementPolicy</span></span>](../resources/unifiedrolemanagementpolicy.md)|<span data-ttu-id="fdf1e-144">A política da atribuição.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-144">The policy for the assignment.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fdf1e-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdf1e-145">JSON representation</span></span>
<span data-ttu-id="fdf1e-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdf1e-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAssignment",
  "id": "String (identifier)",
  "policyId": "String",
  "scopeId": "String",
  "scopeType": "String",
  "roleDefinitionId": "String"
}
```

