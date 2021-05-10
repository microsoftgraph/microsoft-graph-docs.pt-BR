---
title: Tipo de recurso unifiedRoleManagementPolicyNotificationRule
description: Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e4d8952f8ab69ed83aecde96f3bc2804affe24c8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299095"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a><span data-ttu-id="a8b98-104">Tipo de recurso unifiedRoleManagementPolicyNotificationRule</span><span class="sxs-lookup"><span data-stu-id="a8b98-104">unifiedRoleManagementPolicyNotificationRule resource type</span></span>

<span data-ttu-id="a8b98-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8b98-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8b98-106">Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="a8b98-106">A unifiedRoleManagementPolicyNotificationRule specifies the notification rule associated with a role management policy.</span></span> <span data-ttu-id="a8b98-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="a8b98-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="a8b98-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="a8b98-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a8b98-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8b98-109">Properties</span></span>
|<span data-ttu-id="a8b98-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8b98-110">Property</span></span>|<span data-ttu-id="a8b98-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8b98-111">Type</span></span>|<span data-ttu-id="a8b98-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8b98-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b98-113">id</span><span class="sxs-lookup"><span data-stu-id="a8b98-113">id</span></span>|<span data-ttu-id="a8b98-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b98-114">String</span></span>|<span data-ttu-id="a8b98-115">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="a8b98-115">Unique identifier for the rule.</span></span> <span data-ttu-id="a8b98-116">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="a8b98-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="a8b98-117">notificationLevel</span><span class="sxs-lookup"><span data-stu-id="a8b98-117">notificationLevel</span></span>|<span data-ttu-id="a8b98-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b98-118">String</span></span>|<span data-ttu-id="a8b98-119">O nível de notificação.</span><span class="sxs-lookup"><span data-stu-id="a8b98-119">The level of notification.</span></span> <span data-ttu-id="a8b98-120">Um de Nenhum, Crítico, Todos.</span><span class="sxs-lookup"><span data-stu-id="a8b98-120">One of None, Critical, All.</span></span>|
|<span data-ttu-id="a8b98-121">notificationRecipients</span><span class="sxs-lookup"><span data-stu-id="a8b98-121">notificationRecipients</span></span>|<span data-ttu-id="a8b98-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b98-122">String collection</span></span>|<span data-ttu-id="a8b98-123">A lista de recepients de notificação como email.</span><span class="sxs-lookup"><span data-stu-id="a8b98-123">The list of notification recepients like email.</span></span>|
|<span data-ttu-id="a8b98-124">notificationType</span><span class="sxs-lookup"><span data-stu-id="a8b98-124">notificationType</span></span>|<span data-ttu-id="a8b98-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b98-125">String</span></span>|<span data-ttu-id="a8b98-126">O tipo de notificação.</span><span class="sxs-lookup"><span data-stu-id="a8b98-126">The type of notification.</span></span> <span data-ttu-id="a8b98-127">Um de Email.</span><span class="sxs-lookup"><span data-stu-id="a8b98-127">One of Email.</span></span>|
|<span data-ttu-id="a8b98-128">recipientType</span><span class="sxs-lookup"><span data-stu-id="a8b98-128">recipientType</span></span>|<span data-ttu-id="a8b98-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8b98-129">String</span></span>|<span data-ttu-id="a8b98-130">O tipo de destinatário.</span><span class="sxs-lookup"><span data-stu-id="a8b98-130">The type of recipient.</span></span> <span data-ttu-id="a8b98-131">Um dos Solicitadores, Aprovadores, Administradores.</span><span class="sxs-lookup"><span data-stu-id="a8b98-131">One of Requestor, Approver, Admin.</span></span>|
|<span data-ttu-id="a8b98-132">isDefaultRecipientsEnabled</span><span class="sxs-lookup"><span data-stu-id="a8b98-132">isDefaultRecipientsEnabled</span></span>|<span data-ttu-id="a8b98-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="a8b98-133">Boolean</span></span>|<span data-ttu-id="a8b98-134">Se o destinatário padrão está recebendo o email ou não.</span><span class="sxs-lookup"><span data-stu-id="a8b98-134">Whether default recipient is receiving the email or not.</span></span>|
|<span data-ttu-id="a8b98-135">destino</span><span class="sxs-lookup"><span data-stu-id="a8b98-135">target</span></span>|[<span data-ttu-id="a8b98-136">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="a8b98-136">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="a8b98-137">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="a8b98-137">The target for the rule.</span></span> <span data-ttu-id="a8b98-138">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="a8b98-138">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b98-139">Relações</span><span class="sxs-lookup"><span data-stu-id="a8b98-139">Relationships</span></span>
<span data-ttu-id="a8b98-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8b98-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8b98-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8b98-141">JSON representation</span></span>
<span data-ttu-id="a8b98-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8b98-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "baseType": "microsoft.graph.unifiedRoleManagementPolicyRule",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyNotificationRule",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  },
  "notificationType": "String",
  "recipientType": "String",
  "notificationLevel": "String",
  "isDefaultRecipientsEnabled": true,
  "notificationRecipients": [
    "String"
  ]
}
```

