---
title: Tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: efc04b9b65719cbd5952dffb545d371172ab95eb
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137631"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="9df36-103">Tipo de recurso privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9df36-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="9df36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df36-105">Representa as configurações de uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="9df36-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="9df36-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9df36-106">Methods</span></span>

| <span data-ttu-id="9df36-107">Método</span><span class="sxs-lookup"><span data-stu-id="9df36-107">Method</span></span>           | <span data-ttu-id="9df36-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9df36-108">Return Type</span></span>    |<span data-ttu-id="9df36-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9df36-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9df36-110">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9df36-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="9df36-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9df36-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="9df36-112">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="9df36-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="9df36-113">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9df36-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="9df36-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="9df36-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="9df36-115">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="9df36-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="9df36-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9df36-116">Properties</span></span>
| <span data-ttu-id="9df36-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9df36-117">Property</span></span>     | <span data-ttu-id="9df36-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9df36-118">Type</span></span>   |<span data-ttu-id="9df36-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9df36-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9df36-120">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="9df36-120">elevationDuration</span></span>|<span data-ttu-id="9df36-121">duração</span><span class="sxs-lookup"><span data-stu-id="9df36-121">duration</span></span>|<span data-ttu-id="9df36-122">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="9df36-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="9df36-123">id</span><span class="sxs-lookup"><span data-stu-id="9df36-123">id</span></span>|<span data-ttu-id="9df36-124">string</span><span class="sxs-lookup"><span data-stu-id="9df36-124">string</span></span>| <span data-ttu-id="9df36-125">O identificador exclusivo das configurações de função.</span><span class="sxs-lookup"><span data-stu-id="9df36-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="9df36-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9df36-126">Read-only.</span></span>|
|<span data-ttu-id="9df36-127">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="9df36-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="9df36-128">booliano</span><span class="sxs-lookup"><span data-stu-id="9df36-128">boolean</span></span>|<span data-ttu-id="9df36-129">**true** se mfaOnElevation for configurável.</span><span class="sxs-lookup"><span data-stu-id="9df36-129">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="9df36-130">**false** se mfaOnElevation não for configurável.</span><span class="sxs-lookup"><span data-stu-id="9df36-130">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="9df36-131">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="9df36-131">lastGlobalAdmin</span></span>|<span data-ttu-id="9df36-132">booliano</span><span class="sxs-lookup"><span data-stu-id="9df36-132">boolean</span></span>|<span data-ttu-id="9df36-133">Somente para uso interno.</span><span class="sxs-lookup"><span data-stu-id="9df36-133">Internal used only.</span></span>|
|<span data-ttu-id="9df36-134">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="9df36-134">maxElavationDuration</span></span>|<span data-ttu-id="9df36-135">duração</span><span class="sxs-lookup"><span data-stu-id="9df36-135">duration</span></span>|<span data-ttu-id="9df36-136">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="9df36-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="9df36-137">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="9df36-137">mfaOnElevation</span></span>|<span data-ttu-id="9df36-138">booliano</span><span class="sxs-lookup"><span data-stu-id="9df36-138">boolean</span></span>|<span data-ttu-id="9df36-139">**true** se a MFA for necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="9df36-139">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="9df36-140">**false** se a MFA não for necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="9df36-140">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="9df36-141">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="9df36-141">minElevationDuration</span></span>|<span data-ttu-id="9df36-142">duração</span><span class="sxs-lookup"><span data-stu-id="9df36-142">duration</span></span>|<span data-ttu-id="9df36-143">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="9df36-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="9df36-144">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="9df36-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="9df36-145">booliano</span><span class="sxs-lookup"><span data-stu-id="9df36-145">boolean</span></span>|<span data-ttu-id="9df36-146">**true** se enviar notificação para o usuário final quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="9df36-146">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="9df36-147">**false** se não enviar notificação quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="9df36-147">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="9df36-148">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="9df36-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="9df36-149">booliano</span><span class="sxs-lookup"><span data-stu-id="9df36-149">boolean</span></span>|<span data-ttu-id="9df36-150">**true** se as informações de tíquetes são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="9df36-150">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="9df36-151">**false** se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="9df36-151">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="9df36-152">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="9df36-152">approvalOnElevation</span></span>|<span data-ttu-id="9df36-153">booliano</span><span class="sxs-lookup"><span data-stu-id="9df36-153">boolean</span></span>|<span data-ttu-id="9df36-154">**true** se a aprovação for necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="9df36-154">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="9df36-155">**false** se a aprovação não for necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="9df36-155">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="9df36-156">approverIds</span><span class="sxs-lookup"><span data-stu-id="9df36-156">approverIds</span></span>| <span data-ttu-id="9df36-157">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9df36-157">string collection</span></span> |<span data-ttu-id="9df36-158">Lista de IDs de aprovação, se for necessária aprovação para ativação.</span><span class="sxs-lookup"><span data-stu-id="9df36-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9df36-159">Relações</span><span class="sxs-lookup"><span data-stu-id="9df36-159">Relationships</span></span>
<span data-ttu-id="9df36-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9df36-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9df36-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9df36-161">JSON representation</span></span>

<span data-ttu-id="9df36-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9df36-162">Here is a JSON representation of the resource.</span></span>

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


