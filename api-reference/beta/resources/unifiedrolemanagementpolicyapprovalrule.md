---
title: Tipo de recurso unifiedRoleManagementPolicyApprovalRule
description: Um unifiedRoleManagementPolicyApprovalRule especifica a regra de aprovação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0a23087bada876a76658e616add68e404635461f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299061"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a><span data-ttu-id="722a0-104">Tipo de recurso unifiedRoleManagementPolicyApprovalRule</span><span class="sxs-lookup"><span data-stu-id="722a0-104">unifiedRoleManagementPolicyApprovalRule resource type</span></span>

<span data-ttu-id="722a0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="722a0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="722a0-106">Um unifiedRoleManagementPolicyApprovalRule especifica a regra de aprovação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="722a0-106">A unifiedRoleManagementPolicyApprovalRule specifies the approval rule associated with a role management policy.</span></span> <span data-ttu-id="722a0-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="722a0-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="722a0-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="722a0-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="722a0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="722a0-109">Properties</span></span>
|<span data-ttu-id="722a0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="722a0-110">Property</span></span>|<span data-ttu-id="722a0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="722a0-111">Type</span></span>|<span data-ttu-id="722a0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="722a0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="722a0-113">id</span><span class="sxs-lookup"><span data-stu-id="722a0-113">id</span></span>|<span data-ttu-id="722a0-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="722a0-114">String</span></span>|<span data-ttu-id="722a0-115">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="722a0-115">Unique identifier for the rule.</span></span> <span data-ttu-id="722a0-116">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="722a0-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="722a0-117">configuração</span><span class="sxs-lookup"><span data-stu-id="722a0-117">setting</span></span>|[<span data-ttu-id="722a0-118">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="722a0-118">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="722a0-119">A configuração de aprovação da regra.</span><span class="sxs-lookup"><span data-stu-id="722a0-119">The approval setting for the rule.</span></span>|
|<span data-ttu-id="722a0-120">destino</span><span class="sxs-lookup"><span data-stu-id="722a0-120">target</span></span>|[<span data-ttu-id="722a0-121">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="722a0-121">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="722a0-122">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="722a0-122">The target for the rule rule.</span></span> <span data-ttu-id="722a0-123">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="722a0-123">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="722a0-124">Relações</span><span class="sxs-lookup"><span data-stu-id="722a0-124">Relationships</span></span>
<span data-ttu-id="722a0-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="722a0-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="722a0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="722a0-126">JSON representation</span></span>
<span data-ttu-id="722a0-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="722a0-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyApprovalRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "setting": {
    "@odata.type": "microsoft.graph.approvalSettings"
  }
}
```

