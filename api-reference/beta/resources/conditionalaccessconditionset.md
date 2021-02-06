---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2e331a482fce3274463f742ceba6dc111437cd95
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137379"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="9b02d-103">Tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="9b02d-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="9b02d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b02d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b02d-105">Representa o tipo de condições que regem quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="9b02d-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="9b02d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b02d-106">Properties</span></span>

| <span data-ttu-id="9b02d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b02d-107">Property</span></span>     | <span data-ttu-id="9b02d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b02d-108">Type</span></span>        | <span data-ttu-id="9b02d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b02d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b02d-110">applications</span><span class="sxs-lookup"><span data-stu-id="9b02d-110">applications</span></span>|[<span data-ttu-id="9b02d-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="9b02d-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="9b02d-112">Aplicativos e ações do usuário incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="9b02d-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b02d-113">Required.</span></span> |
|<span data-ttu-id="9b02d-114">usuários</span><span class="sxs-lookup"><span data-stu-id="9b02d-114">users</span></span>|[<span data-ttu-id="9b02d-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="9b02d-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="9b02d-116">Usuários, grupos e funções incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="9b02d-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b02d-117">Required.</span></span> |
|<span data-ttu-id="9b02d-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="9b02d-118">clientAppTypes</span></span>|<span data-ttu-id="9b02d-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b02d-119">String collection</span></span>| <span data-ttu-id="9b02d-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-120">Client application types included in the policy.</span></span> <span data-ttu-id="9b02d-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="9b02d-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="9b02d-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="9b02d-122">deviceStates</span></span>|[<span data-ttu-id="9b02d-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="9b02d-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="9b02d-124">Estados do dispositivo na política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-124">Device states in the policy.</span></span> |
|<span data-ttu-id="9b02d-125">devices</span><span class="sxs-lookup"><span data-stu-id="9b02d-125">devices</span></span>|[<span data-ttu-id="9b02d-126">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="9b02d-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="9b02d-127">Dispositivos na política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-127">Devices in the policy.</span></span> |
|<span data-ttu-id="9b02d-128">locations</span><span class="sxs-lookup"><span data-stu-id="9b02d-128">locations</span></span>|[<span data-ttu-id="9b02d-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="9b02d-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="9b02d-130">Locais incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="9b02d-131">platforms</span><span class="sxs-lookup"><span data-stu-id="9b02d-131">platforms</span></span>|[<span data-ttu-id="9b02d-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="9b02d-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="9b02d-133">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="9b02d-134">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="9b02d-134">signInRiskLevels</span></span>|<span data-ttu-id="9b02d-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b02d-135">String collection</span></span>| <span data-ttu-id="9b02d-136">Níveis de risco de login incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-136">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="9b02d-137">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="9b02d-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="9b02d-138">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="9b02d-138">userRiskLevels</span></span>|<span data-ttu-id="9b02d-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b02d-139">String collection</span></span>| <span data-ttu-id="9b02d-140">Níveis de risco do usuário incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="9b02d-140">User risk levels included in the policy.</span></span> <span data-ttu-id="9b02d-141">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="9b02d-141">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="9b02d-142">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="9b02d-142">**Note:**</span></span> 

><span data-ttu-id="9b02d-143">**clientAppType** `modern` será preterido e substituído por `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="9b02d-143">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="9b02d-144">**clientAppType** `easUnsupported` será preterido em favor do que inclui plataformas compatíveis e sem suporte `exchangeActiveSync` do EAS.</span><span class="sxs-lookup"><span data-stu-id="9b02d-144">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="9b02d-145">Estamos preterindo a **condição deviceStates** e ela pode ser removida no futuro.</span><span class="sxs-lookup"><span data-stu-id="9b02d-145">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="9b02d-146">No futuro, use a **condição de dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="9b02d-146">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="9b02d-147">Relações</span><span class="sxs-lookup"><span data-stu-id="9b02d-147">Relationships</span></span>

<span data-ttu-id="9b02d-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b02d-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b02d-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b02d-149">JSON representation</span></span>

<span data-ttu-id="9b02d-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b02d-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
    "devices",
    "locations",
    "platforms",
    "signInRiskLevels"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessConditionSet",
  "baseType": null
}-->

```json
{
  "applications": {"@odata.type": "microsoft.graph.conditionalAccessApplications"},
  "users": {"@odata.type": "microsoft.graph.conditionalAccessUsers"},
  "clientAppTypes": ["String"],
  "deviceStates": {"@odata.type": "microsoft.graph.conditionalAccessDeviceStates"},
  "devices": {"@odata.type": "microsoft.graph.conditionalAccessDevices"},
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


