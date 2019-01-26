---
title: tipo de recurso de privilegedRoleSettings
description: Representa as configurações para uma função privilegiada.
localization_priority: Normal
ms.openlocfilehash: 673327e3c83a4111eb469ca48550836433dbdf0a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577148"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="5e241-103">tipo de recurso de privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5e241-103">privilegedRoleSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e241-104">Representa as configurações para uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="5e241-104">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="5e241-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e241-105">Methods</span></span>

| <span data-ttu-id="5e241-106">Método</span><span class="sxs-lookup"><span data-stu-id="5e241-106">Method</span></span>           | <span data-ttu-id="5e241-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5e241-107">Return Type</span></span>    |<span data-ttu-id="5e241-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e241-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e241-109">Obter privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5e241-109">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="5e241-110">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5e241-110">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="5e241-111">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="5e241-111">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="5e241-112">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5e241-112">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="5e241-113">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="5e241-113">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="5e241-114">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="5e241-114">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="5e241-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e241-115">Properties</span></span>
| <span data-ttu-id="5e241-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e241-116">Property</span></span>     | <span data-ttu-id="5e241-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e241-117">Type</span></span>   |<span data-ttu-id="5e241-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e241-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e241-119">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="5e241-119">elevationDuration</span></span>| <span data-ttu-id="5e241-120">Cadeia de caracteres (timestamp)</span><span class="sxs-lookup"><span data-stu-id="5e241-120">String (timestamp)</span></span> |<span data-ttu-id="5e241-121">A duração quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="5e241-121">The duration when the role is activated.</span></span>|
|<span data-ttu-id="5e241-122">id</span><span class="sxs-lookup"><span data-stu-id="5e241-122">id</span></span>| <span data-ttu-id="5e241-123">cadeia de caracteres (identificador)</span><span class="sxs-lookup"><span data-stu-id="5e241-123">string (identifier)</span></span>| <span data-ttu-id="5e241-124">O identificador exclusivo para as configurações de função.</span><span class="sxs-lookup"><span data-stu-id="5e241-124">The unique identifier for the role settings.</span></span> <span data-ttu-id="5e241-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e241-125">Read-only.</span></span>|
|<span data-ttu-id="5e241-126">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="5e241-126">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="5e241-127">booliano</span><span class="sxs-lookup"><span data-stu-id="5e241-127">boolean</span></span>|<span data-ttu-id="5e241-128">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="5e241-128">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="5e241-129">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="5e241-129">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="5e241-130">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="5e241-130">lastGlobalAdmin</span></span>|<span data-ttu-id="5e241-131">booliano</span><span class="sxs-lookup"><span data-stu-id="5e241-131">boolean</span></span>|<span data-ttu-id="5e241-132">Interno usado apenas.</span><span class="sxs-lookup"><span data-stu-id="5e241-132">Internal used only.</span></span>|
|<span data-ttu-id="5e241-133">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="5e241-133">maxElavationDuration</span></span>| <span data-ttu-id="5e241-134">cadeia de caracteres (identificador)</span><span class="sxs-lookup"><span data-stu-id="5e241-134">string (identifier)</span></span>| |<span data-ttu-id="5e241-135">Duração máxima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="5e241-135">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="5e241-136">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="5e241-136">mfaOnElevation</span></span>|<span data-ttu-id="5e241-137">booliano</span><span class="sxs-lookup"><span data-stu-id="5e241-137">boolean</span></span>|<span data-ttu-id="5e241-138">**true** se MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5e241-138">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="5e241-139">**false** se MFA não é necessário para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5e241-139">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="5e241-140">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="5e241-140">minElevationDuration</span></span>|<span data-ttu-id="5e241-141">cadeia de caracteres (identificador)</span><span class="sxs-lookup"><span data-stu-id="5e241-141">string (identifier)</span></span>||<span data-ttu-id="5e241-142">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="5e241-142">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="5e241-143">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="5e241-143">notificationToUserOnElevation</span></span>|<span data-ttu-id="5e241-144">booliano</span><span class="sxs-lookup"><span data-stu-id="5e241-144">boolean</span></span>|<span data-ttu-id="5e241-145">**True** se enviar notificação ao usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="5e241-145">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="5e241-146">**False** se não enviar notificação quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="5e241-146">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="5e241-147">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="5e241-147">ticketingInfoOnElevation</span></span>|<span data-ttu-id="5e241-148">booliano</span><span class="sxs-lookup"><span data-stu-id="5e241-148">boolean</span></span>|<span data-ttu-id="5e241-149">**true** se as informações de tickets são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5e241-149">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="5e241-150">**false** se as informações de tickets não são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5e241-150">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="5e241-151">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="5e241-151">approvalOnElevation</span></span>|<span data-ttu-id="5e241-152">booliano</span><span class="sxs-lookup"><span data-stu-id="5e241-152">boolean</span></span>|<span data-ttu-id="5e241-153">**true** se a aprovação é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5e241-153">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="5e241-154">**false** se a aprovação não é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="5e241-154">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="5e241-155">approverIds</span><span class="sxs-lookup"><span data-stu-id="5e241-155">approverIds</span></span>| <span data-ttu-id="5e241-156">String collection</span><span class="sxs-lookup"><span data-stu-id="5e241-156">String collection</span></span> |<span data-ttu-id="5e241-157">Lista de ids de aprovação, se a aprovação é necessária para a ativação.</span><span class="sxs-lookup"><span data-stu-id="5e241-157">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e241-158">Relações</span><span class="sxs-lookup"><span data-stu-id="5e241-158">Relationships</span></span>
<span data-ttu-id="5e241-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5e241-159">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e241-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e241-160">JSON representation</span></span>

<span data-ttu-id="5e241-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e241-161">Here is a JSON representation of the resource.</span></span>

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
  "approverIds": [ "String (identifier)" ]
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
