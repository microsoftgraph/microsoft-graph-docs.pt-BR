---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 763fe78508a61461f824e618867abe96c1afd348
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122599"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="51e36-103">tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="51e36-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="51e36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51e36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e36-105">Representa o tipo de condições que controlam quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="51e36-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="51e36-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51e36-106">Properties</span></span>

| <span data-ttu-id="51e36-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51e36-107">Property</span></span>     | <span data-ttu-id="51e36-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="51e36-108">Type</span></span>        | <span data-ttu-id="51e36-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e36-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51e36-110">Emprego</span><span class="sxs-lookup"><span data-stu-id="51e36-110">applications</span></span>|[<span data-ttu-id="51e36-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="51e36-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="51e36-112">Aplicativos e ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="51e36-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="51e36-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e36-113">Required.</span></span> |
|<span data-ttu-id="51e36-114">usuários</span><span class="sxs-lookup"><span data-stu-id="51e36-114">users</span></span>|[<span data-ttu-id="51e36-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="51e36-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="51e36-116">Usuários, grupos e funções incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="51e36-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="51e36-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e36-117">Required.</span></span> |
|<span data-ttu-id="51e36-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="51e36-118">clientAppTypes</span></span>|<span data-ttu-id="51e36-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e36-119">String collection</span></span>| <span data-ttu-id="51e36-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="51e36-120">Client application types included in the policy.</span></span> <span data-ttu-id="51e36-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="51e36-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="51e36-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="51e36-122">deviceStates</span></span>|[<span data-ttu-id="51e36-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="51e36-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="51e36-124">Estados do dispositivo na política.</span><span class="sxs-lookup"><span data-stu-id="51e36-124">Device states in the policy.</span></span> |
|<span data-ttu-id="51e36-125">dispositivos</span><span class="sxs-lookup"><span data-stu-id="51e36-125">devices</span></span>|[<span data-ttu-id="51e36-126">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="51e36-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="51e36-127">Dispositivos na política.</span><span class="sxs-lookup"><span data-stu-id="51e36-127">Devices in the policy.</span></span> |
|<span data-ttu-id="51e36-128">locations</span><span class="sxs-lookup"><span data-stu-id="51e36-128">locations</span></span>|[<span data-ttu-id="51e36-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="51e36-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="51e36-130">Locais incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="51e36-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="51e36-131">plataformas</span><span class="sxs-lookup"><span data-stu-id="51e36-131">platforms</span></span>|[<span data-ttu-id="51e36-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="51e36-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="51e36-133">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="51e36-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="51e36-134">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="51e36-134">signInRiskLevels</span></span>|<span data-ttu-id="51e36-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e36-135">String collection</span></span>| <span data-ttu-id="51e36-136">Níveis de risco de entrada incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="51e36-136">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="51e36-137">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="51e36-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="51e36-138">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="51e36-138">userRiskLevels</span></span>|<span data-ttu-id="51e36-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e36-139">String collection</span></span>| <span data-ttu-id="51e36-140">Níveis de risco do usuário incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="51e36-140">User risk levels included in the policy.</span></span> <span data-ttu-id="51e36-141">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="51e36-141">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="51e36-142">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="51e36-142">**Note:**</span></span> 

><span data-ttu-id="51e36-143">**clientAppType** `modern` será preterido e substituído por `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="51e36-143">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="51e36-144">**clientAppType** `easUnsupported` será preterido em favor do `exchangeActiveSync` que inclui EAS plataformas suportadas e não suportadas.</span><span class="sxs-lookup"><span data-stu-id="51e36-144">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="51e36-145">Estamos preterindo a condição **deviceStates** e ela poderá ser removida no futuro.</span><span class="sxs-lookup"><span data-stu-id="51e36-145">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="51e36-146">Em frente, use a condição **dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="51e36-146">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="51e36-147">Relações</span><span class="sxs-lookup"><span data-stu-id="51e36-147">Relationships</span></span>

<span data-ttu-id="51e36-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51e36-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51e36-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51e36-149">JSON representation</span></span>

<span data-ttu-id="51e36-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51e36-150">The following is a JSON representation of the resource.</span></span>

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
