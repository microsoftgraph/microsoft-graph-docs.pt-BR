---
title: Tipo de recurso policyRoot
description: Uma nova associação de propriedades de navegação para unifiedRoleManagementPolicy e unifiedRoleManagementPolicyAssignment para policyRoot.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 85c334c52ab2bb196bcfce24610414a0843f898a
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299053"
---
# <a name="policyroot-resource-type"></a><span data-ttu-id="9322e-103">Tipo de recurso policyRoot</span><span class="sxs-lookup"><span data-stu-id="9322e-103">policyRoot resource type</span></span>

<span data-ttu-id="9322e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9322e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9322e-105">Uma nova associação de propriedades de navegação para unifiedRoleManagementPolicy e unifiedRoleManagementPolicyAssignment para policyRoot.</span><span class="sxs-lookup"><span data-stu-id="9322e-105">A new navigation properties binding for unifiedRoleManagementPolicy and unifiedRoleManagementPolicyAssignment to policyRoot.</span></span>

## <a name="methods"></a><span data-ttu-id="9322e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9322e-106">Methods</span></span>
|<span data-ttu-id="9322e-107">Método</span><span class="sxs-lookup"><span data-stu-id="9322e-107">Method</span></span>|<span data-ttu-id="9322e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9322e-108">Return type</span></span>|<span data-ttu-id="9322e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9322e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9322e-110">Listar roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="9322e-110">List roleManagementPolicies</span></span>](../api/policyroot-list-rolemanagementpolicies.md)|<span data-ttu-id="9322e-111">[Coleção unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="9322e-111">[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection</span></span>|<span data-ttu-id="9322e-112">Obter os recursos unifiedRoleManagementPolicy da propriedade de navegação roleManagementPolicies.</span><span class="sxs-lookup"><span data-stu-id="9322e-112">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>|
|[<span data-ttu-id="9322e-113">Listar roleManagementPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="9322e-113">List roleManagementPolicyAssignments</span></span>](../api/policyroot-list-rolemanagementpolicyassignments.md)|<span data-ttu-id="9322e-114">[Coleção unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="9322e-114">[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection</span></span>|<span data-ttu-id="9322e-115">Obter os recursos de navegação unifiedRoleManagementPolicyAssignment da propriedade de navegação roleManagementPolicyAssignments.</span><span class="sxs-lookup"><span data-stu-id="9322e-115">Get the unifiedRoleManagementPolicyAssignment resources from the roleManagementPolicyAssignments navigation property.</span></span>|

<!--
## Properties
|Property|Type|Description|
|:---|:---|:---|


## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleManagementPolicies|[unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) collection|Represents the role management policies.|
|roleManagementPolicyAssignments|[unifiedRoleManagementPolicyAssignment](../resources/unifiedrolemanagementpolicyassignment.md) collection|Represents the role management policy assignments.|
-->

## <a name="json-representation"></a><span data-ttu-id="9322e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9322e-116">JSON representation</span></span>
<span data-ttu-id="9322e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9322e-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyRoot"
}
```

