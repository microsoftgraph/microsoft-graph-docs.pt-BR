---
title: tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ed87787ca8016f1dde7711304a1da1fc977c641b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965709"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="98d93-103">tipo de recurso privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="98d93-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98d93-104">Representa as configurações de uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="98d93-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="98d93-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="98d93-105">Methods</span></span>

| <span data-ttu-id="98d93-106">Método</span><span class="sxs-lookup"><span data-stu-id="98d93-106">Method</span></span>           | <span data-ttu-id="98d93-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="98d93-107">Return Type</span></span>    |<span data-ttu-id="98d93-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="98d93-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98d93-109">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="98d93-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="98d93-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="98d93-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="98d93-111">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="98d93-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="98d93-112">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="98d93-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="98d93-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="98d93-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="98d93-114">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="98d93-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="98d93-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98d93-115">Properties</span></span>
| <span data-ttu-id="98d93-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98d93-116">Property</span></span>     | <span data-ttu-id="98d93-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="98d93-117">Type</span></span>   |<span data-ttu-id="98d93-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="98d93-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98d93-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="98d93-119">elevationDuration</span></span>|<span data-ttu-id="98d93-120">duration</span><span class="sxs-lookup"><span data-stu-id="98d93-120">duration</span></span>|<span data-ttu-id="98d93-121">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="98d93-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="98d93-122">id</span><span class="sxs-lookup"><span data-stu-id="98d93-122">id</span></span>|<span data-ttu-id="98d93-123">string</span><span class="sxs-lookup"><span data-stu-id="98d93-123">string</span></span>| <span data-ttu-id="98d93-124">O identificador exclusivo das configurações de função.</span><span class="sxs-lookup"><span data-stu-id="98d93-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="98d93-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98d93-125">Read-only.</span></span>|
|<span data-ttu-id="98d93-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="98d93-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="98d93-127">booliano</span><span class="sxs-lookup"><span data-stu-id="98d93-127">boolean</span></span>|<span data-ttu-id="98d93-128">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="98d93-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="98d93-129">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="98d93-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="98d93-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="98d93-130">lastGlobalAdmin</span></span>|<span data-ttu-id="98d93-131">booliano</span><span class="sxs-lookup"><span data-stu-id="98d93-131">boolean</span></span>|<span data-ttu-id="98d93-132">Somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="98d93-132">Internal used only.</span></span>|
|<span data-ttu-id="98d93-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="98d93-133">maxElavationDuration</span></span>|<span data-ttu-id="98d93-134">duration</span><span class="sxs-lookup"><span data-stu-id="98d93-134">duration</span></span>|<span data-ttu-id="98d93-135">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="98d93-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="98d93-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="98d93-136">mfaOnElevation</span></span>|<span data-ttu-id="98d93-137">booliano</span><span class="sxs-lookup"><span data-stu-id="98d93-137">boolean</span></span>|<span data-ttu-id="98d93-138">**true** se a MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="98d93-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="98d93-139">**false** se a MFA não é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="98d93-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="98d93-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="98d93-140">minElevationDuration</span></span>|<span data-ttu-id="98d93-141">duration</span><span class="sxs-lookup"><span data-stu-id="98d93-141">duration</span></span>|<span data-ttu-id="98d93-142">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="98d93-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="98d93-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="98d93-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="98d93-144">booliano</span><span class="sxs-lookup"><span data-stu-id="98d93-144">boolean</span></span>|<span data-ttu-id="98d93-145">**true** se enviar notificação para o usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="98d93-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="98d93-146">**false** se não enviar notificações quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="98d93-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="98d93-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="98d93-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="98d93-148">booliano</span><span class="sxs-lookup"><span data-stu-id="98d93-148">boolean</span></span>|<span data-ttu-id="98d93-149">**true** se as informações de tíquete são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="98d93-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="98d93-150">**false** se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="98d93-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="98d93-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="98d93-151">approvalOnElevation</span></span>|<span data-ttu-id="98d93-152">booliano</span><span class="sxs-lookup"><span data-stu-id="98d93-152">boolean</span></span>|<span data-ttu-id="98d93-153">**true** se a aprovação é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="98d93-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="98d93-154">**false** se a aprovação não é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="98d93-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="98d93-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="98d93-155">approverIds</span></span>| <span data-ttu-id="98d93-156">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="98d93-156">string collection</span></span> |<span data-ttu-id="98d93-157">Lista de IDs de aprovação, se a aprovação for necessária para ativação.</span><span class="sxs-lookup"><span data-stu-id="98d93-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98d93-158">Relações</span><span class="sxs-lookup"><span data-stu-id="98d93-158">Relationships</span></span>
<span data-ttu-id="98d93-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98d93-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="98d93-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98d93-160">JSON representation</span></span>

<span data-ttu-id="98d93-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98d93-161">Here is a JSON representation of the resource.</span></span>

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
