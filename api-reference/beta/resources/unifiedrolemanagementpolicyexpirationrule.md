---
title: Tipo de recurso unifiedRoleManagementPolicyExpirationRule
description: Uma unifiedRoleManagementPolicyExpirationRule especifica a regra de habilitação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 610ecd2e861ac672d0b211e313132caa6946d8ff
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299058"
---
# <a name="unifiedrolemanagementpolicyexpirationrule-resource-type"></a><span data-ttu-id="b6179-104">Tipo de recurso unifiedRoleManagementPolicyExpirationRule</span><span class="sxs-lookup"><span data-stu-id="b6179-104">unifiedRoleManagementPolicyExpirationRule resource type</span></span>

<span data-ttu-id="b6179-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6179-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6179-106">Uma unifiedRoleManagementPolicyExpirationRule especifica a regra de habilitação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="b6179-106">A unifiedRoleManagementPolicyExpirationRule specifies the enablement rule associated with a role management policy.</span></span> <span data-ttu-id="b6179-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="b6179-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="b6179-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="b6179-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b6179-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6179-109">Properties</span></span>
|<span data-ttu-id="b6179-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6179-110">Property</span></span>|<span data-ttu-id="b6179-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6179-111">Type</span></span>|<span data-ttu-id="b6179-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6179-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6179-113">id</span><span class="sxs-lookup"><span data-stu-id="b6179-113">id</span></span>|<span data-ttu-id="b6179-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6179-114">String</span></span>|<span data-ttu-id="b6179-115">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="b6179-115">Unique identifier for the rule.</span></span> <span data-ttu-id="b6179-116">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b6179-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="b6179-117">isExpirationRequired</span><span class="sxs-lookup"><span data-stu-id="b6179-117">isExpirationRequired</span></span>|<span data-ttu-id="b6179-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6179-118">Boolean</span></span>|<span data-ttu-id="b6179-119">Indica se a expiração é necessária para qualificação ou atribuição.</span><span class="sxs-lookup"><span data-stu-id="b6179-119">Indicates if expiration is required for eligibility or assignment.</span></span>|
|<span data-ttu-id="b6179-120">maximumDuration</span><span class="sxs-lookup"><span data-stu-id="b6179-120">maximumDuration</span></span>|<span data-ttu-id="b6179-121">Duration</span><span class="sxs-lookup"><span data-stu-id="b6179-121">Duration</span></span>|<span data-ttu-id="b6179-122">A duração máxima permitida para a elegência ou atribuição que não é permanente.</span><span class="sxs-lookup"><span data-stu-id="b6179-122">The maximum duration allowed for eligiblity or assignment which is not permanent.</span></span>|
|<span data-ttu-id="b6179-123">destino</span><span class="sxs-lookup"><span data-stu-id="b6179-123">target</span></span>|[<span data-ttu-id="b6179-124">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="b6179-124">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="b6179-125">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="b6179-125">The target for the rule.</span></span> <span data-ttu-id="b6179-126">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="b6179-126">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6179-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b6179-127">Relationships</span></span>
<span data-ttu-id="b6179-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6179-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6179-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6179-129">JSON representation</span></span>
<span data-ttu-id="b6179-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6179-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "isExpirationRequired": "Boolean",
  "maximumDuration": "String (duration)"
}
```

