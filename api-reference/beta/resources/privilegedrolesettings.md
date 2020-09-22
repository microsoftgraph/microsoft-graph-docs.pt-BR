---
title: tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: 7a082804309799c946f05f21d37d92b2eded7d13
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070503"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="0992e-103">tipo de recurso privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="0992e-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="0992e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0992e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0992e-105">Representa as configurações de uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="0992e-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="0992e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0992e-106">Methods</span></span>

| <span data-ttu-id="0992e-107">Método</span><span class="sxs-lookup"><span data-stu-id="0992e-107">Method</span></span>           | <span data-ttu-id="0992e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0992e-108">Return Type</span></span>    |<span data-ttu-id="0992e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0992e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0992e-110">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="0992e-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="0992e-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="0992e-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="0992e-112">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="0992e-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="0992e-113">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="0992e-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="0992e-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="0992e-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="0992e-115">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="0992e-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="0992e-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0992e-116">Properties</span></span>
| <span data-ttu-id="0992e-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0992e-117">Property</span></span>     | <span data-ttu-id="0992e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="0992e-118">Type</span></span>   |<span data-ttu-id="0992e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0992e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0992e-120">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="0992e-120">elevationDuration</span></span>|<span data-ttu-id="0992e-121">duration</span><span class="sxs-lookup"><span data-stu-id="0992e-121">duration</span></span>|<span data-ttu-id="0992e-122">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="0992e-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="0992e-123">id</span><span class="sxs-lookup"><span data-stu-id="0992e-123">id</span></span>|<span data-ttu-id="0992e-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0992e-124">string</span></span>| <span data-ttu-id="0992e-125">O identificador exclusivo das configurações de função.</span><span class="sxs-lookup"><span data-stu-id="0992e-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="0992e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0992e-126">Read-only.</span></span>|
|<span data-ttu-id="0992e-127">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="0992e-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="0992e-128">booliano</span><span class="sxs-lookup"><span data-stu-id="0992e-128">boolean</span></span>|<span data-ttu-id="0992e-129">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="0992e-129">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="0992e-130">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="0992e-130">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="0992e-131">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="0992e-131">lastGlobalAdmin</span></span>|<span data-ttu-id="0992e-132">booliano</span><span class="sxs-lookup"><span data-stu-id="0992e-132">boolean</span></span>|<span data-ttu-id="0992e-133">Somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="0992e-133">Internal used only.</span></span>|
|<span data-ttu-id="0992e-134">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="0992e-134">maxElavationDuration</span></span>|<span data-ttu-id="0992e-135">duration</span><span class="sxs-lookup"><span data-stu-id="0992e-135">duration</span></span>|<span data-ttu-id="0992e-136">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="0992e-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="0992e-137">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="0992e-137">mfaOnElevation</span></span>|<span data-ttu-id="0992e-138">booliano</span><span class="sxs-lookup"><span data-stu-id="0992e-138">boolean</span></span>|<span data-ttu-id="0992e-139">**true** se a MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="0992e-139">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="0992e-140">**false** se a MFA não é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="0992e-140">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="0992e-141">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="0992e-141">minElevationDuration</span></span>|<span data-ttu-id="0992e-142">duration</span><span class="sxs-lookup"><span data-stu-id="0992e-142">duration</span></span>|<span data-ttu-id="0992e-143">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="0992e-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="0992e-144">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="0992e-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="0992e-145">booliano</span><span class="sxs-lookup"><span data-stu-id="0992e-145">boolean</span></span>|<span data-ttu-id="0992e-146">**true** se enviar notificação para o usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="0992e-146">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="0992e-147">**false** se não enviar notificações quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="0992e-147">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="0992e-148">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="0992e-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="0992e-149">booliano</span><span class="sxs-lookup"><span data-stu-id="0992e-149">boolean</span></span>|<span data-ttu-id="0992e-150">**true** se as informações de tíquete são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="0992e-150">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="0992e-151">**false** se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="0992e-151">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="0992e-152">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="0992e-152">approvalOnElevation</span></span>|<span data-ttu-id="0992e-153">booliano</span><span class="sxs-lookup"><span data-stu-id="0992e-153">boolean</span></span>|<span data-ttu-id="0992e-154">**true** se a aprovação é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="0992e-154">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="0992e-155">**false** se a aprovação não é necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="0992e-155">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="0992e-156">approverIds</span><span class="sxs-lookup"><span data-stu-id="0992e-156">approverIds</span></span>| <span data-ttu-id="0992e-157">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0992e-157">string collection</span></span> |<span data-ttu-id="0992e-158">Lista de IDs de aprovação, se a aprovação for necessária para ativação.</span><span class="sxs-lookup"><span data-stu-id="0992e-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0992e-159">Relações</span><span class="sxs-lookup"><span data-stu-id="0992e-159">Relationships</span></span>
<span data-ttu-id="0992e-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0992e-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0992e-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0992e-161">JSON representation</span></span>

<span data-ttu-id="0992e-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0992e-162">Here is a JSON representation of the resource.</span></span>

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


