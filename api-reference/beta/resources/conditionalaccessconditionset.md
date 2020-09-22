---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba88e9e5fd67bba5dd88fe323f3140bdbebff479
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994292"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="8ff78-103">tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="8ff78-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="8ff78-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff78-105">Representa o tipo de condições que controlam quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="8ff78-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="8ff78-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ff78-106">Properties</span></span>

| <span data-ttu-id="8ff78-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ff78-107">Property</span></span>     | <span data-ttu-id="8ff78-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ff78-108">Type</span></span>        | <span data-ttu-id="8ff78-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ff78-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ff78-110">Emprego</span><span class="sxs-lookup"><span data-stu-id="8ff78-110">applications</span></span>|[<span data-ttu-id="8ff78-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="8ff78-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="8ff78-112">Aplicativos e ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="8ff78-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff78-113">Required.</span></span> |
|<span data-ttu-id="8ff78-114">usuários</span><span class="sxs-lookup"><span data-stu-id="8ff78-114">users</span></span>|[<span data-ttu-id="8ff78-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="8ff78-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="8ff78-116">Usuários, grupos e funções incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="8ff78-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ff78-117">Required.</span></span> |
|<span data-ttu-id="8ff78-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="8ff78-118">clientAppTypes</span></span>|<span data-ttu-id="8ff78-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff78-119">String collection</span></span>| <span data-ttu-id="8ff78-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-120">Client application types included in the policy.</span></span> <span data-ttu-id="8ff78-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="8ff78-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="8ff78-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="8ff78-122">deviceStates</span></span>|[<span data-ttu-id="8ff78-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="8ff78-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="8ff78-124">Estados do dispositivo na política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-124">Device states in the policy.</span></span> |
|<span data-ttu-id="8ff78-125">dispositivos</span><span class="sxs-lookup"><span data-stu-id="8ff78-125">devices</span></span>|[<span data-ttu-id="8ff78-126">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="8ff78-126">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="8ff78-127">Dispositivos na política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-127">Devices in the policy.</span></span> |
|<span data-ttu-id="8ff78-128">locations</span><span class="sxs-lookup"><span data-stu-id="8ff78-128">locations</span></span>|[<span data-ttu-id="8ff78-129">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="8ff78-129">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="8ff78-130">Locais incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-130">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="8ff78-131">plataformas</span><span class="sxs-lookup"><span data-stu-id="8ff78-131">platforms</span></span>|[<span data-ttu-id="8ff78-132">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="8ff78-132">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="8ff78-133">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-133">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="8ff78-134">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="8ff78-134">signInRiskLevels</span></span>|<span data-ttu-id="8ff78-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff78-135">String collection</span></span>| <span data-ttu-id="8ff78-136">Níveis de risco de entrada incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-136">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="8ff78-137">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8ff78-137">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="8ff78-138">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="8ff78-138">userRiskLevels</span></span>|<span data-ttu-id="8ff78-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ff78-139">String collection</span></span>| <span data-ttu-id="8ff78-140">Níveis de risco do usuário incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="8ff78-140">User risk levels included in the policy.</span></span> <span data-ttu-id="8ff78-141">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8ff78-141">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

><span data-ttu-id="8ff78-142">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="8ff78-142">**Note:**</span></span> 

><span data-ttu-id="8ff78-143">**clientAppType** `modern` será preterido e substituído por `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="8ff78-143">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> 

><span data-ttu-id="8ff78-144">**clientAppType** `easUnsupported` será preterido em favor do `exchangeActiveSync` que inclui EAS plataformas suportadas e não suportadas.</span><span class="sxs-lookup"><span data-stu-id="8ff78-144">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> 

><span data-ttu-id="8ff78-145">Estamos preterindo a condição **deviceStates** e ela poderá ser removida no futuro.</span><span class="sxs-lookup"><span data-stu-id="8ff78-145">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="8ff78-146">Em frente, use a condição **dispositivos** .</span><span class="sxs-lookup"><span data-stu-id="8ff78-146">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="8ff78-147">Relações</span><span class="sxs-lookup"><span data-stu-id="8ff78-147">Relationships</span></span>

<span data-ttu-id="8ff78-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ff78-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ff78-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ff78-149">JSON representation</span></span>

<span data-ttu-id="8ff78-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ff78-150">The following is a JSON representation of the resource.</span></span>

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


