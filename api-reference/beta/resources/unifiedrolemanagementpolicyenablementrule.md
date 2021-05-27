---
title: Tipo de recurso unifiedRoleManagementPolicyEnablementRule
description: Uma unifiedRoleManagementPolicyEnablementRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bf3ef8e25026c72aab36a9c2fb6241f5bef950da
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680679"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a><span data-ttu-id="dccd7-104">Tipo de recurso unifiedRoleManagementPolicyEnablementRule</span><span class="sxs-lookup"><span data-stu-id="dccd7-104">unifiedRoleManagementPolicyEnablementRule resource type</span></span>

<span data-ttu-id="dccd7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dccd7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dccd7-106">Uma unifiedRoleManagementPolicyEnablementRule especifica a regra de habilitação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="dccd7-106">A unifiedRoleManagementPolicyEnablementRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="dccd7-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="dccd7-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="dccd7-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="dccd7-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dccd7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dccd7-109">Properties</span></span>
|<span data-ttu-id="dccd7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dccd7-110">Property</span></span>|<span data-ttu-id="dccd7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dccd7-111">Type</span></span>|<span data-ttu-id="dccd7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dccd7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dccd7-113">enabledRules</span><span class="sxs-lookup"><span data-stu-id="dccd7-113">enabledRules</span></span>|<span data-ttu-id="dccd7-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dccd7-114">String collection</span></span>|<span data-ttu-id="dccd7-115">As regras que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="dccd7-115">The rules which are enabled.</span></span> <span data-ttu-id="dccd7-116">Os valores permitidos são MultifactorAuthentication, Justification, Ticketing.</span><span class="sxs-lookup"><span data-stu-id="dccd7-116">Allowed values are MultifactorAuthentication, Justification, Ticketing.</span></span>|
|<span data-ttu-id="dccd7-117">id</span><span class="sxs-lookup"><span data-stu-id="dccd7-117">id</span></span>|<span data-ttu-id="dccd7-118">String</span><span class="sxs-lookup"><span data-stu-id="dccd7-118">String</span></span>|<span data-ttu-id="dccd7-119">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="dccd7-119">Unique identifier for the rule.</span></span> <span data-ttu-id="dccd7-120">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="dccd7-120">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="dccd7-121">destino</span><span class="sxs-lookup"><span data-stu-id="dccd7-121">target</span></span>|[<span data-ttu-id="dccd7-122">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="dccd7-122">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="dccd7-123">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="dccd7-123">The target for the rule.</span></span> <span data-ttu-id="dccd7-124">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="dccd7-124">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dccd7-125">Relações</span><span class="sxs-lookup"><span data-stu-id="dccd7-125">Relationships</span></span>
<span data-ttu-id="dccd7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dccd7-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dccd7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dccd7-127">JSON representation</span></span>
<span data-ttu-id="dccd7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dccd7-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyEnablementRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "enabledRules": [
    "String"
  ]
}
```

