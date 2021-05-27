---
title: Tipo de recurso unifiedRoleManagementPolicyApprovalRule
description: Um unifiedRoleManagementPolicyApprovalRule especifica a regra de aprovação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 41d9cac01f48d8dcdd59513718053611b023a3a8
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680700"
---
# <a name="unifiedrolemanagementpolicyapprovalrule-resource-type"></a><span data-ttu-id="b2132-104">Tipo de recurso unifiedRoleManagementPolicyApprovalRule</span><span class="sxs-lookup"><span data-stu-id="b2132-104">unifiedRoleManagementPolicyApprovalRule resource type</span></span>

<span data-ttu-id="b2132-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2132-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2132-106">Um unifiedRoleManagementPolicyApprovalRule especifica a regra de aprovação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="b2132-106">A unifiedRoleManagementPolicyApprovalRule specifies the approval rule associated with a role management policy.</span></span> <span data-ttu-id="b2132-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="b2132-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="b2132-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="b2132-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b2132-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2132-109">Properties</span></span>
|<span data-ttu-id="b2132-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2132-110">Property</span></span>|<span data-ttu-id="b2132-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2132-111">Type</span></span>|<span data-ttu-id="b2132-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2132-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2132-113">id</span><span class="sxs-lookup"><span data-stu-id="b2132-113">id</span></span>|<span data-ttu-id="b2132-114">String</span><span class="sxs-lookup"><span data-stu-id="b2132-114">String</span></span>|<span data-ttu-id="b2132-115">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="b2132-115">Unique identifier for the rule.</span></span> <span data-ttu-id="b2132-116">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b2132-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="b2132-117">configuração</span><span class="sxs-lookup"><span data-stu-id="b2132-117">setting</span></span>|[<span data-ttu-id="b2132-118">approvalSettings</span><span class="sxs-lookup"><span data-stu-id="b2132-118">approvalSettings</span></span>](../resources/approvalsettings.md)|<span data-ttu-id="b2132-119">A configuração de aprovação da regra.</span><span class="sxs-lookup"><span data-stu-id="b2132-119">The approval setting for the rule.</span></span>|
|<span data-ttu-id="b2132-120">destino</span><span class="sxs-lookup"><span data-stu-id="b2132-120">target</span></span>|[<span data-ttu-id="b2132-121">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="b2132-121">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="b2132-122">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="b2132-122">The target for the rule rule.</span></span> <span data-ttu-id="b2132-123">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b2132-123">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2132-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b2132-124">Relationships</span></span>
<span data-ttu-id="b2132-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2132-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2132-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2132-126">JSON representation</span></span>
<span data-ttu-id="b2132-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2132-127">The following is a JSON representation of the resource.</span></span>
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

