---
title: Tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: a1f20455ffcc818aa1b1edf784d6990d68b7556b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962561"
---
# <a name="privilegedrolesettings-resource-type"></a><span data-ttu-id="6b45a-103">Tipo de recurso privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6b45a-103">privilegedRoleSettings resource type</span></span>

<span data-ttu-id="6b45a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b45a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b45a-105">Representa as configurações de uma função privilegiada.</span><span class="sxs-lookup"><span data-stu-id="6b45a-105">Represents the settings for a privileged role.</span></span>


## <a name="methods"></a><span data-ttu-id="6b45a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b45a-106">Methods</span></span>

| <span data-ttu-id="6b45a-107">Método</span><span class="sxs-lookup"><span data-stu-id="6b45a-107">Method</span></span>           | <span data-ttu-id="6b45a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b45a-108">Return Type</span></span>    |<span data-ttu-id="6b45a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b45a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b45a-110">Get privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6b45a-110">Get privilegedRoleSettings</span></span>](../api/privilegedrolesettings-get.md) | [<span data-ttu-id="6b45a-111">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6b45a-111">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="6b45a-112">Ler propriedades e relações do objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="6b45a-112">Read properties and relationships of privilegedRoleSettings object.</span></span>|
|[<span data-ttu-id="6b45a-113">Atualizar privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6b45a-113">Update privilegedRoleSettings</span></span>](../api/privilegedrolesettings-update.md) | [<span data-ttu-id="6b45a-114">privilegedRoleSettings</span><span class="sxs-lookup"><span data-stu-id="6b45a-114">privilegedRoleSettings</span></span>](privilegedrolesettings.md) |<span data-ttu-id="6b45a-115">Atualize o objeto privilegedRoleSettings.</span><span class="sxs-lookup"><span data-stu-id="6b45a-115">Update privilegedRoleSettings object.</span></span>|
## <a name="properties"></a><span data-ttu-id="6b45a-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b45a-116">Properties</span></span>
| <span data-ttu-id="6b45a-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b45a-117">Property</span></span>     | <span data-ttu-id="6b45a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b45a-118">Type</span></span>   |<span data-ttu-id="6b45a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b45a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b45a-120">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="6b45a-120">elevationDuration</span></span>|<span data-ttu-id="6b45a-121">duração</span><span class="sxs-lookup"><span data-stu-id="6b45a-121">duration</span></span>|<span data-ttu-id="6b45a-122">A duração quando a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="6b45a-122">The duration when the role is activated.</span></span>|
|<span data-ttu-id="6b45a-123">id</span><span class="sxs-lookup"><span data-stu-id="6b45a-123">id</span></span>|<span data-ttu-id="6b45a-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b45a-124">string</span></span>| <span data-ttu-id="6b45a-125">O identificador exclusivo para as configurações de função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-125">The unique identifier for the role settings.</span></span> <span data-ttu-id="6b45a-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b45a-126">Read-only.</span></span>|
|<span data-ttu-id="6b45a-127">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="6b45a-127">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="6b45a-128">booliano</span><span class="sxs-lookup"><span data-stu-id="6b45a-128">boolean</span></span>|<span data-ttu-id="6b45a-129">`true` se **mfaOnElevation** for configurável.</span><span class="sxs-lookup"><span data-stu-id="6b45a-129">`true` if **mfaOnElevation** is configurable.</span></span> <span data-ttu-id="6b45a-130">`false` se **mfaOnElevation** não for configurável.</span><span class="sxs-lookup"><span data-stu-id="6b45a-130">`false` if **mfaOnElevation** is not configurable.</span></span>|
|<span data-ttu-id="6b45a-131">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="6b45a-131">lastGlobalAdmin</span></span>|<span data-ttu-id="6b45a-132">booliano</span><span class="sxs-lookup"><span data-stu-id="6b45a-132">boolean</span></span>|<span data-ttu-id="6b45a-133">Somente uso interno.</span><span class="sxs-lookup"><span data-stu-id="6b45a-133">Internal used only.</span></span>|
|<span data-ttu-id="6b45a-134">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="6b45a-134">maxElavationDuration</span></span>|<span data-ttu-id="6b45a-135">duração</span><span class="sxs-lookup"><span data-stu-id="6b45a-135">duration</span></span>|<span data-ttu-id="6b45a-136">Duração máxima da função ativada.</span><span class="sxs-lookup"><span data-stu-id="6b45a-136">Maximal duration for the activated role.</span></span>|
|<span data-ttu-id="6b45a-137">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="6b45a-137">mfaOnElevation</span></span>|<span data-ttu-id="6b45a-138">booliano</span><span class="sxs-lookup"><span data-stu-id="6b45a-138">boolean</span></span>|<span data-ttu-id="6b45a-139">`true` se o MFA for necessário para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-139">`true` if MFA is required to activate the role.</span></span> <span data-ttu-id="6b45a-140">`false` se o MFA não for necessário para ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-140">`false` if MFA is not required to activate the role.</span></span>|
|<span data-ttu-id="6b45a-141">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="6b45a-141">minElevationDuration</span></span>|<span data-ttu-id="6b45a-142">duração</span><span class="sxs-lookup"><span data-stu-id="6b45a-142">duration</span></span>|<span data-ttu-id="6b45a-143">Duração mínima para a função ativada.</span><span class="sxs-lookup"><span data-stu-id="6b45a-143">Minimal duration for the activated role.</span></span>|
|<span data-ttu-id="6b45a-144">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="6b45a-144">notificationToUserOnElevation</span></span>|<span data-ttu-id="6b45a-145">booliano</span><span class="sxs-lookup"><span data-stu-id="6b45a-145">boolean</span></span>|<span data-ttu-id="6b45a-146">`true` se enviar notificação ao usuário final quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="6b45a-146">`true` if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="6b45a-147">`false` se não enviar notificação quando a função for ativada.</span><span class="sxs-lookup"><span data-stu-id="6b45a-147">`false` if do not send notification when the role is activated.</span></span>|
|<span data-ttu-id="6b45a-148">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="6b45a-148">ticketingInfoOnElevation</span></span>|<span data-ttu-id="6b45a-149">booliano</span><span class="sxs-lookup"><span data-stu-id="6b45a-149">boolean</span></span>|<span data-ttu-id="6b45a-150">`true` se as informações de tíquete são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-150">`true` if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="6b45a-151">`false` se as informações de tíquete não são necessárias ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-151">`false` if the ticketing information is not required when activate the role.</span></span>|
|<span data-ttu-id="6b45a-152">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="6b45a-152">approvalOnElevation</span></span>|<span data-ttu-id="6b45a-153">booliano</span><span class="sxs-lookup"><span data-stu-id="6b45a-153">boolean</span></span>|<span data-ttu-id="6b45a-154">`true` se a aprovação for necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-154">`true` if the approval is required when activate the role.</span></span> <span data-ttu-id="6b45a-155">`false` se a aprovação não for necessária ao ativar a função.</span><span class="sxs-lookup"><span data-stu-id="6b45a-155">`false` if the approval is not required when activate the role.</span></span>|
|<span data-ttu-id="6b45a-156">approverIds</span><span class="sxs-lookup"><span data-stu-id="6b45a-156">approverIds</span></span>| <span data-ttu-id="6b45a-157">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b45a-157">string collection</span></span> |<span data-ttu-id="6b45a-158">Lista de IDs de Aprovação, se a aprovação for necessária para ativação.</span><span class="sxs-lookup"><span data-stu-id="6b45a-158">List of Approval ids, if approval is required for activation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b45a-159">Relações</span><span class="sxs-lookup"><span data-stu-id="6b45a-159">Relationships</span></span>
<span data-ttu-id="6b45a-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b45a-160">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b45a-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b45a-161">JSON representation</span></span>

<span data-ttu-id="6b45a-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b45a-162">Here is a JSON representation of the resource.</span></span>

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


