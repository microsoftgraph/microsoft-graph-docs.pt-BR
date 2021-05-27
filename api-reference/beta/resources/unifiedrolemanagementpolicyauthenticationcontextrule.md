---
title: Tipo de recurso unifiedRoleManagementPolicyAuthenticationContextRule
description: Uma unifiedRoleManagementPolicyAuthenticationContextRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5e3db8812b58b8276ab2fdd977e110f30a874c9b
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680693"
---
# <a name="unifiedrolemanagementpolicyauthenticationcontextrule-resource-type"></a><span data-ttu-id="b1563-104">Tipo de recurso unifiedRoleManagementPolicyAuthenticationContextRule</span><span class="sxs-lookup"><span data-stu-id="b1563-104">unifiedRoleManagementPolicyAuthenticationContextRule resource type</span></span>

<span data-ttu-id="b1563-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1563-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1563-106">Uma unifiedRoleManagementPolicyAuthenticationContextRule especifica a regra de habilitação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="b1563-106">A unifiedRoleManagementPolicyAuthenticationContextRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="b1563-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="b1563-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="b1563-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="b1563-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b1563-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1563-109">Properties</span></span>
|<span data-ttu-id="b1563-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1563-110">Property</span></span>|<span data-ttu-id="b1563-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1563-111">Type</span></span>|<span data-ttu-id="b1563-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1563-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1563-113">claimValue</span><span class="sxs-lookup"><span data-stu-id="b1563-113">claimValue</span></span>|<span data-ttu-id="b1563-114">String</span><span class="sxs-lookup"><span data-stu-id="b1563-114">String</span></span>|<span data-ttu-id="b1563-115">Valor da declaração de contexto de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b1563-115">Value of the authentication context claim.</span></span>|
|<span data-ttu-id="b1563-116">id</span><span class="sxs-lookup"><span data-stu-id="b1563-116">id</span></span>|<span data-ttu-id="b1563-117">String</span><span class="sxs-lookup"><span data-stu-id="b1563-117">String</span></span>|<span data-ttu-id="b1563-118">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="b1563-118">Unique identifier for the rule.</span></span> <span data-ttu-id="b1563-119">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b1563-119">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="b1563-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b1563-120">isEnabled</span></span>|<span data-ttu-id="b1563-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1563-121">Boolean</span></span>|<span data-ttu-id="b1563-122">Indica se a configuração está habilitada.</span><span class="sxs-lookup"><span data-stu-id="b1563-122">Indicates if the setting is enabled.</span></span>|
|<span data-ttu-id="b1563-123">destino</span><span class="sxs-lookup"><span data-stu-id="b1563-123">target</span></span>|[<span data-ttu-id="b1563-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="b1563-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="b1563-125">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="b1563-125">The target for the rule.</span></span> <span data-ttu-id="b1563-126">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b1563-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1563-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b1563-127">Relationships</span></span>
<span data-ttu-id="b1563-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1563-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1563-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1563-129">JSON representation</span></span>
<span data-ttu-id="b1563-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1563-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyAuthenticationContextRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isEnabled": "Boolean",
  "claimValue": "String"
}
```

