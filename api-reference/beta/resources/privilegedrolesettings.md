---
title: tipo de recurso de privilegedRoleSettings
description: Representa as configurações para uma função privilegiada.
ms.openlocfilehash: 14b4919d653de80c97f06aff507c011162c3c0e4
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2018
ms.locfileid: "27041223"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="12e36-103">tipo de recurso de privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="12e36-103">privilegedRoleSettings resource type</span></span>

> <span data-ttu-id="12e36-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="12e36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12e36-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12e36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12e36-106">Representa as configurações para uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="12e36-106">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="12e36-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="12e36-107">Methods</span></span>

| <span data-ttu-id="12e36-108">Método</span><span class="sxs-lookup"><span data-stu-id="12e36-108">Method</span></span>           | <span data-ttu-id="12e36-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12e36-109">Return Type</span></span>    |<span data-ttu-id="12e36-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e36-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12e36-111">Obter privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="12e36-111">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="12e36-112">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="12e36-112">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="12e36-113">Leia as propriedades e os relacionamentos do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="12e36-113">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="12e36-114">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="12e36-114">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="12e36-115">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="12e36-115">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="12e36-116">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="12e36-116">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="12e36-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12e36-117">Properties</span></span>
| <span data-ttu-id="12e36-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12e36-118">Property</span></span>     | <span data-ttu-id="12e36-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="12e36-119">Type</span></span>   |<span data-ttu-id="12e36-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e36-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e36-121">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="12e36-121">elevationDuration</span></span>|<span data-ttu-id="12e36-122">duration</span><span class="sxs-lookup"><span data-stu-id="12e36-122">duration</span></span>|<span data-ttu-id="12e36-123">A duração quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="12e36-123">The duration when the role is activated.</span></span>|
|<span data-ttu-id="12e36-124">id</span><span class="sxs-lookup"><span data-stu-id="12e36-124">id</span></span>|<span data-ttu-id="12e36-125">string</span><span class="sxs-lookup"><span data-stu-id="12e36-125">string</span></span>| <span data-ttu-id="12e36-126">O identificador exclusivo para as configurações de função.</span><span class="sxs-lookup"><span data-stu-id="12e36-126">The unique identifier for the role settings.</span></span> <span data-ttu-id="12e36-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12e36-127">Read-only.</span></span>|
|<span data-ttu-id="12e36-128">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="12e36-128">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="12e36-129">booliano</span><span class="sxs-lookup"><span data-stu-id="12e36-129">boolean</span></span>|<span data-ttu-id="12e36-130">**true** se mfaOnElevation é configurável.</span><span class="sxs-lookup"><span data-stu-id="12e36-130">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="12e36-131">**false** se mfaOnElevation não é configurável.</span><span class="sxs-lookup"><span data-stu-id="12e36-131">**false** if mfaOnElevation is not configurable.</span></span>|
|<span data-ttu-id="12e36-132">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="12e36-132">lastGlobalAdmin</span></span>|<span data-ttu-id="12e36-133">booliano</span><span class="sxs-lookup"><span data-stu-id="12e36-133">boolean</span></span>|<span data-ttu-id="12e36-134">Interno usado apenas.</span><span class="sxs-lookup"><span data-stu-id="12e36-134">Internal used only.</span></span>|
|<span data-ttu-id="12e36-135">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="12e36-135">maxElavationDuration</span></span>|<span data-ttu-id="12e36-136">duration</span><span class="sxs-lookup"><span data-stu-id="12e36-136">duration</span></span>|<span data-ttu-id="12e36-137">Duração máxima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="12e36-137">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="12e36-138">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="12e36-138">mfaOnElevation</span></span>|<span data-ttu-id="12e36-139">booliano</span><span class="sxs-lookup"><span data-stu-id="12e36-139">boolean</span></span>|<span data-ttu-id="12e36-140">**true** se MFA é necessária para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="12e36-140">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="12e36-141">**false** se MFA não é necessário para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="12e36-141">**false** if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="12e36-142">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="12e36-142">minElevationDuration</span></span>|<span data-ttu-id="12e36-143">duration</span><span class="sxs-lookup"><span data-stu-id="12e36-143">duration</span></span>|<span data-ttu-id="12e36-144">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="12e36-144">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="12e36-145">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="12e36-145">notificationToUserOnElevation</span></span>|<span data-ttu-id="12e36-146">booliano</span><span class="sxs-lookup"><span data-stu-id="12e36-146">boolean</span></span>|<span data-ttu-id="12e36-147">**True** se enviar notificação ao usuário final quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="12e36-147">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="12e36-148">**False** se não enviar notificação quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="12e36-148">**false** if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="12e36-149">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="12e36-149">ticketingInfoOnElevation</span></span>|<span data-ttu-id="12e36-150">booliano</span><span class="sxs-lookup"><span data-stu-id="12e36-150">boolean</span></span>|<span data-ttu-id="12e36-151">**true** se as informações de tickets são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="12e36-151">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="12e36-152">**false** se as informações de tickets não são necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="12e36-152">**false** if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="12e36-153">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="12e36-153">approvalOnElevation</span></span>|<span data-ttu-id="12e36-154">booliano</span><span class="sxs-lookup"><span data-stu-id="12e36-154">boolean</span></span>|<span data-ttu-id="12e36-155">**true** se a aprovação é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="12e36-155">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="12e36-156">**false** se a aprovação não é necessária quando ativar a função.</span><span class="sxs-lookup"><span data-stu-id="12e36-156">**false** if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="12e36-157">approverIds</span><span class="sxs-lookup"><span data-stu-id="12e36-157">approverIds</span></span>|<span data-ttu-id="12e36-158">array</span><span class="sxs-lookup"><span data-stu-id="12e36-158">array</span></span>|<span data-ttu-id="12e36-159">Lista de ids de aprovação, se a aprovação é necessária para a ativação.</span><span class="sxs-lookup"><span data-stu-id="12e36-159">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12e36-160">Relações</span><span class="sxs-lookup"><span data-stu-id="12e36-160">Relationships</span></span>
<span data-ttu-id="12e36-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12e36-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="12e36-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12e36-162">JSON representation</span></span>

<span data-ttu-id="12e36-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12e36-163">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->