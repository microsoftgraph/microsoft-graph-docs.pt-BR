---
title: tipo de recurso de privilegedRoleSettings
description: Representa as configurações para uma função privilegiada.
localization_priority: Normal
ms.openlocfilehash: 7d4c14065defc63190d1d25b435c734b9f219e36
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642776"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="6e87a-103">tipo de recurso de privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6e87a-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e87a-104">Representa as configurações para uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="6e87a-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="6e87a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e87a-105">Methods</span></span>

| <span data-ttu-id="6e87a-106">Método</span><span class="sxs-lookup"><span data-stu-id="6e87a-106">Method</span></span>           | <span data-ttu-id="6e87a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6e87a-107">Return Type</span></span>    |<span data-ttu-id="6e87a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e87a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e87a-109">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6e87a-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="6e87a-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6e87a-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="6e87a-111">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="6e87a-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="6e87a-112">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6e87a-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="6e87a-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6e87a-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="6e87a-114">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="6e87a-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="6e87a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e87a-115">Properties</span></span>
| <span data-ttu-id="6e87a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e87a-116">Property</span></span>     | <span data-ttu-id="6e87a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e87a-117">Type</span></span>   |<span data-ttu-id="6e87a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e87a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e87a-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="6e87a-119">elevationDuration</span></span>|<span data-ttu-id="6e87a-120">duration</span><span class="sxs-lookup"><span data-stu-id="6e87a-120">duration</span></span>|<span data-ttu-id="6e87a-121">A duração quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="6e87a-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="6e87a-122">id</span><span class="sxs-lookup"><span data-stu-id="6e87a-122">id</span></span>|<span data-ttu-id="6e87a-123">string</span><span class="sxs-lookup"><span data-stu-id="6e87a-123">string</span></span>| <span data-ttu-id="6e87a-124">O identificador exclusivo para as configurações de função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="6e87a-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e87a-125">Read-only.</span></span>|
|<span data-ttu-id="6e87a-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="6e87a-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="6e87a-127">boolean</span><span class="sxs-lookup"><span data-stu-id="6e87a-127">boolean</span></span>|<span data-ttu-id="6e87a-128">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="6e87a-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="6e87a-129">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="6e87a-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="6e87a-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="6e87a-130">lastGlobalAdmin</span></span>|<span data-ttu-id="6e87a-131">boolean</span><span class="sxs-lookup"><span data-stu-id="6e87a-131">boolean</span></span>|<span data-ttu-id="6e87a-132">Interno usado apenas.</span><span class="sxs-lookup"><span data-stu-id="6e87a-132">Internal used only.</span></span>|
|<span data-ttu-id="6e87a-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="6e87a-133">maxElavationDuration</span></span>|<span data-ttu-id="6e87a-134">duration</span><span class="sxs-lookup"><span data-stu-id="6e87a-134">duration</span></span>|<span data-ttu-id="6e87a-135">Duração máxima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="6e87a-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="6e87a-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="6e87a-136">mfaOnElevation</span></span>|<span data-ttu-id="6e87a-137">boolean</span><span class="sxs-lookup"><span data-stu-id="6e87a-137">boolean</span></span>|<span data-ttu-id="6e87a-138">**true** se MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="6e87a-139">**false** se MFA não é necessário para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="6e87a-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="6e87a-140">minElevationDuration</span></span>|<span data-ttu-id="6e87a-141">duration</span><span class="sxs-lookup"><span data-stu-id="6e87a-141">duration</span></span>|<span data-ttu-id="6e87a-142">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="6e87a-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="6e87a-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="6e87a-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="6e87a-144">boolean</span><span class="sxs-lookup"><span data-stu-id="6e87a-144">boolean</span></span>|<span data-ttu-id="6e87a-145">**True** se enviar notificação ao usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="6e87a-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="6e87a-146">**False** se não enviar notificação quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="6e87a-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="6e87a-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="6e87a-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="6e87a-148">boolean</span><span class="sxs-lookup"><span data-stu-id="6e87a-148">boolean</span></span>|<span data-ttu-id="6e87a-149">**true** se as informações de tickets são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="6e87a-150">**false** se as informações de tickets não são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="6e87a-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="6e87a-151">approvalOnElevation</span></span>|<span data-ttu-id="6e87a-152">boolean</span><span class="sxs-lookup"><span data-stu-id="6e87a-152">boolean</span></span>|<span data-ttu-id="6e87a-153">**true** se a aprovação é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="6e87a-154">**false** se a aprovação não é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6e87a-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="6e87a-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="6e87a-155">approverIds</span></span>|<span data-ttu-id="6e87a-156">array</span><span class="sxs-lookup"><span data-stu-id="6e87a-156">array</span></span>|<span data-ttu-id="6e87a-157">Lista de ids de aprovação, se a aprovação é necessária para a ativação.</span><span class="sxs-lookup"><span data-stu-id="6e87a-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e87a-158">Relações</span><span class="sxs-lookup"><span data-stu-id="6e87a-158">Relationships</span></span>
<span data-ttu-id="6e87a-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e87a-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e87a-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e87a-160">JSON representation</span></span>

<span data-ttu-id="6e87a-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e87a-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": []
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
