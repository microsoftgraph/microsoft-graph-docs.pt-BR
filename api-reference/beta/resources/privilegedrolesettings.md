---
title: tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
ms.openlocfilehash: 6500d5a51fcedce97d71c1c4022c7d941de27b83
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344204"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="119e7-103">tipo de recurso privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="119e7-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="119e7-104">Representa as configurações de uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="119e7-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="119e7-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="119e7-105">Methods</span></span>

| <span data-ttu-id="119e7-106">Método</span><span class="sxs-lookup"><span data-stu-id="119e7-106">Method</span></span>           | <span data-ttu-id="119e7-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="119e7-107">Return Type</span></span>    |<span data-ttu-id="119e7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="119e7-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="119e7-109">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="119e7-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="119e7-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="119e7-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="119e7-111">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="119e7-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="119e7-112">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="119e7-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="119e7-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="119e7-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="119e7-114">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="119e7-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="119e7-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="119e7-115">Properties</span></span>
| <span data-ttu-id="119e7-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="119e7-116">Property</span></span>     | <span data-ttu-id="119e7-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="119e7-117">Type</span></span>   |<span data-ttu-id="119e7-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="119e7-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="119e7-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="119e7-119">elevationDuration</span></span>|<span data-ttu-id="119e7-120">duration</span><span class="sxs-lookup"><span data-stu-id="119e7-120">duration</span></span>|<span data-ttu-id="119e7-121">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="119e7-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="119e7-122">id</span><span class="sxs-lookup"><span data-stu-id="119e7-122">id</span></span>|<span data-ttu-id="119e7-123">string</span><span class="sxs-lookup"><span data-stu-id="119e7-123">string</span></span>| <span data-ttu-id="119e7-124">O identificador exclusivo das configurações de função.</span><span class="sxs-lookup"><span data-stu-id="119e7-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="119e7-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="119e7-125">Read-only.</span></span>|
|<span data-ttu-id="119e7-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="119e7-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="119e7-127">booliano</span><span class="sxs-lookup"><span data-stu-id="119e7-127">boolean</span></span>|<span data-ttu-id="119e7-128">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="119e7-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="119e7-129">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="119e7-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="119e7-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="119e7-130">lastGlobalAdmin</span></span>|<span data-ttu-id="119e7-131">booliano</span><span class="sxs-lookup"><span data-stu-id="119e7-131">boolean</span></span>|<span data-ttu-id="119e7-132">Somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="119e7-132">Internal used only.</span></span>|
|<span data-ttu-id="119e7-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="119e7-133">maxElavationDuration</span></span>|<span data-ttu-id="119e7-134">duration</span><span class="sxs-lookup"><span data-stu-id="119e7-134">duration</span></span>|<span data-ttu-id="119e7-135">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="119e7-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="119e7-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="119e7-136">mfaOnElevation</span></span>|<span data-ttu-id="119e7-137">booliano</span><span class="sxs-lookup"><span data-stu-id="119e7-137">boolean</span></span>|<span data-ttu-id="119e7-138">**true** se a MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="119e7-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="119e7-139">**false** se a MFA não é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="119e7-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="119e7-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="119e7-140">minElevationDuration</span></span>|<span data-ttu-id="119e7-141">duration</span><span class="sxs-lookup"><span data-stu-id="119e7-141">duration</span></span>|<span data-ttu-id="119e7-142">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="119e7-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="119e7-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="119e7-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="119e7-144">booliano</span><span class="sxs-lookup"><span data-stu-id="119e7-144">boolean</span></span>|<span data-ttu-id="119e7-145">**true** se enviar notificação para o usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="119e7-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="119e7-146">**false** se não enviar notificações quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="119e7-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="119e7-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="119e7-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="119e7-148">booliano</span><span class="sxs-lookup"><span data-stu-id="119e7-148">boolean</span></span>|<span data-ttu-id="119e7-149">**true** se as informações de tíquete são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="119e7-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="119e7-150">**false** se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="119e7-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="119e7-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="119e7-151">approvalOnElevation</span></span>|<span data-ttu-id="119e7-152">booliano</span><span class="sxs-lookup"><span data-stu-id="119e7-152">boolean</span></span>|<span data-ttu-id="119e7-153">**true** se a aprovação é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="119e7-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="119e7-154">**false** se a aprovação não é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="119e7-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="119e7-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="119e7-155">approverIds</span></span>| <span data-ttu-id="119e7-156">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="119e7-156">string collection</span></span> |<span data-ttu-id="119e7-157">Lista de IDs de aprovação, se a aprovação for necessária para ativação.</span><span class="sxs-lookup"><span data-stu-id="119e7-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="119e7-158">Relações</span><span class="sxs-lookup"><span data-stu-id="119e7-158">Relationships</span></span>
<span data-ttu-id="119e7-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="119e7-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="119e7-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="119e7-160">JSON representation</span></span>

<span data-ttu-id="119e7-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="119e7-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
