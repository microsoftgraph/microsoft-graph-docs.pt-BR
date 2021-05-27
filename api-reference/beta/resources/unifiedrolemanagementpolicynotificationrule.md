---
title: Tipo de recurso unifiedRoleManagementPolicyNotificationRule
description: Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função. Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c4392055d199e444acefa497a009cf5b71cb8cda
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680196"
---
# <a name="unifiedrolemanagementpolicynotificationrule-resource-type"></a><span data-ttu-id="4bae2-104">Tipo de recurso unifiedRoleManagementPolicyNotificationRule</span><span class="sxs-lookup"><span data-stu-id="4bae2-104">unifiedRoleManagementPolicyNotificationRule resource type</span></span>

<span data-ttu-id="4bae2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bae2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4bae2-106">Um unifiedRoleManagementPolicyNotificationRule especifica a regra de notificação associada a uma política de gerenciamento de função.</span><span class="sxs-lookup"><span data-stu-id="4bae2-106">A unifiedRoleManagementPolicyNotificationRule specifies the notification rule associated with a role management policy.</span></span> <span data-ttu-id="4bae2-107">Ele é derivado de microsoft.graph.unifiedRoleManagementPolicyRule.</span><span class="sxs-lookup"><span data-stu-id="4bae2-107">It is derived from microsoft.graph.unifiedRoleManagementPolicyRule.</span></span>

<span data-ttu-id="4bae2-108">Herda [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span><span class="sxs-lookup"><span data-stu-id="4bae2-108">Inherits from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4bae2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bae2-109">Properties</span></span>
|<span data-ttu-id="4bae2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bae2-110">Property</span></span>|<span data-ttu-id="4bae2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bae2-111">Type</span></span>|<span data-ttu-id="4bae2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bae2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bae2-113">id</span><span class="sxs-lookup"><span data-stu-id="4bae2-113">id</span></span>|<span data-ttu-id="4bae2-114">String</span><span class="sxs-lookup"><span data-stu-id="4bae2-114">String</span></span>|<span data-ttu-id="4bae2-115">Identificador exclusivo da regra.</span><span class="sxs-lookup"><span data-stu-id="4bae2-115">Unique identifier for the rule.</span></span> <span data-ttu-id="4bae2-116">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="4bae2-116">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|
|<span data-ttu-id="4bae2-117">notificationLevel</span><span class="sxs-lookup"><span data-stu-id="4bae2-117">notificationLevel</span></span>|<span data-ttu-id="4bae2-118">String</span><span class="sxs-lookup"><span data-stu-id="4bae2-118">String</span></span>|<span data-ttu-id="4bae2-119">O nível de notificação.</span><span class="sxs-lookup"><span data-stu-id="4bae2-119">The level of notification.</span></span> <span data-ttu-id="4bae2-120">Um de Nenhum, Crítico, Todos.</span><span class="sxs-lookup"><span data-stu-id="4bae2-120">One of None, Critical, All.</span></span>|
|<span data-ttu-id="4bae2-121">notificationRecipients</span><span class="sxs-lookup"><span data-stu-id="4bae2-121">notificationRecipients</span></span>|<span data-ttu-id="4bae2-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bae2-122">String collection</span></span>|<span data-ttu-id="4bae2-123">A lista de recepients de notificação como email.</span><span class="sxs-lookup"><span data-stu-id="4bae2-123">The list of notification recepients like email.</span></span>|
|<span data-ttu-id="4bae2-124">notificationType</span><span class="sxs-lookup"><span data-stu-id="4bae2-124">notificationType</span></span>|<span data-ttu-id="4bae2-125">String</span><span class="sxs-lookup"><span data-stu-id="4bae2-125">String</span></span>|<span data-ttu-id="4bae2-126">O tipo de notificação.</span><span class="sxs-lookup"><span data-stu-id="4bae2-126">The type of notification.</span></span> <span data-ttu-id="4bae2-127">Um de Email.</span><span class="sxs-lookup"><span data-stu-id="4bae2-127">One of Email.</span></span>|
|<span data-ttu-id="4bae2-128">recipientType</span><span class="sxs-lookup"><span data-stu-id="4bae2-128">recipientType</span></span>|<span data-ttu-id="4bae2-129">String</span><span class="sxs-lookup"><span data-stu-id="4bae2-129">String</span></span>|<span data-ttu-id="4bae2-130">O tipo de destinatário.</span><span class="sxs-lookup"><span data-stu-id="4bae2-130">The type of recipient.</span></span> <span data-ttu-id="4bae2-131">Um dos Solicitadores, Aprovadores, Administradores.</span><span class="sxs-lookup"><span data-stu-id="4bae2-131">One of Requestor, Approver, Admin.</span></span>|
|<span data-ttu-id="4bae2-132">isDefaultRecipientsEnabled</span><span class="sxs-lookup"><span data-stu-id="4bae2-132">isDefaultRecipientsEnabled</span></span>|<span data-ttu-id="4bae2-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bae2-133">Boolean</span></span>|<span data-ttu-id="4bae2-134">Se o destinatário padrão está recebendo o email ou não.</span><span class="sxs-lookup"><span data-stu-id="4bae2-134">Whether default recipient is receiving the email or not.</span></span>|
|<span data-ttu-id="4bae2-135">destino</span><span class="sxs-lookup"><span data-stu-id="4bae2-135">target</span></span>|[<span data-ttu-id="4bae2-136">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="4bae2-136">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="4bae2-137">O destino da regra.</span><span class="sxs-lookup"><span data-stu-id="4bae2-137">The target for the rule.</span></span> <span data-ttu-id="4bae2-138">Herdado [de unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span><span class="sxs-lookup"><span data-stu-id="4bae2-138">Inherited from [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bae2-139">Relações</span><span class="sxs-lookup"><span data-stu-id="4bae2-139">Relationships</span></span>
<span data-ttu-id="4bae2-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bae2-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bae2-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bae2-141">JSON representation</span></span>
<span data-ttu-id="4bae2-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4bae2-142">The following is a JSON representation of the resource.</span></span>
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

