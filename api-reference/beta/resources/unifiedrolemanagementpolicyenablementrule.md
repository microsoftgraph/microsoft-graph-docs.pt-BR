---
title: Tipo de recurso unifiedRoleManagementPolicyEnablementRule
description: Uma unifiedRoleManagementPolicyEnablementRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2cb5770f2fdd50aaf5e82d7c1f8fba505a47151
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299059"
---
# <a name="unifiedrolemanagementpolicyenablementrule-resource-type"></a><span data-ttu-id="091b9-104">Tipo de recurso unifiedRoleManagementPolicyEnablementRule</span><span class="sxs-lookup"><span data-stu-id="091b9-104">unifiedRoleManagementPolicyEnablementRule resource type</span></span>

<span data-ttu-id="091b9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="091b9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="091b9-106">Uma unifiedRoleManagementPolicyEnablementRule especifica a regra de habilitação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="091b9-106">A unifiedRoleManagementPolicyEnablementRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="091b9-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="091b9-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="091b9-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="091b9-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="091b9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="091b9-109">Properties</span></span>
|<span data-ttu-id="091b9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="091b9-110">Property</span></span>|<span data-ttu-id="091b9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="091b9-111">Type</span></span>|<span data-ttu-id="091b9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="091b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="091b9-113">enabledRules</span><span class="sxs-lookup"><span data-stu-id="091b9-113">enabledRules</span></span>|<span data-ttu-id="091b9-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="091b9-114">String collection</span></span>|<span data-ttu-id="091b9-115">As regras que estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="091b9-115">The rules which are enabled.</span></span> <span data-ttu-id="091b9-116">Os valores permitidos são MultifactorAuthentication, Justification, Ticketing.</span><span class="sxs-lookup"><span data-stu-id="091b9-116">Allowed values are MultifactorAuthentication, Justification, Ticketing.</span></span>|
|<span data-ttu-id="091b9-117">id</span><span class="sxs-lookup"><span data-stu-id="091b9-117">id</span></span>|<span data-ttu-id="091b9-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="091b9-118">String</span></span>|<span data-ttu-id="091b9-119">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="091b9-119">Unique identifier for the rule.</span></span> <span data-ttu-id="091b9-120">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="091b9-120">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="091b9-121">destino</span><span class="sxs-lookup"><span data-stu-id="091b9-121">target</span></span>|[<span data-ttu-id="091b9-122">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="091b9-122">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="091b9-123">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="091b9-123">The target for the rule.</span></span> <span data-ttu-id="091b9-124">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="091b9-124">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="091b9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="091b9-125">Relationships</span></span>
<span data-ttu-id="091b9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="091b9-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="091b9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="091b9-127">JSON representation</span></span>
<span data-ttu-id="091b9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="091b9-128">The following is a JSON representation of the resource.</span></span>
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

