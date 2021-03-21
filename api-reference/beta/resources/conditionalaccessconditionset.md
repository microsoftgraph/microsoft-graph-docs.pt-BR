---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 162943a5f2d51744ae37d6644f8a01eafb31c259
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961287"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="de6bd-103">Tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="de6bd-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="de6bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de6bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de6bd-105">Representa o tipo de condições que regem quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="de6bd-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="de6bd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de6bd-106">Properties</span></span>

| <span data-ttu-id="de6bd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de6bd-107">Property</span></span>     | <span data-ttu-id="de6bd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="de6bd-108">Type</span></span>        | <span data-ttu-id="de6bd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de6bd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de6bd-110">applications</span><span class="sxs-lookup"><span data-stu-id="de6bd-110">applications</span></span>|[<span data-ttu-id="de6bd-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="de6bd-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="de6bd-112">Aplicativos e ações do usuário incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="de6bd-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6bd-113">Required.</span></span> |
|<span data-ttu-id="de6bd-114">usuários</span><span class="sxs-lookup"><span data-stu-id="de6bd-114">users</span></span>|[<span data-ttu-id="de6bd-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="de6bd-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="de6bd-116">Usuários, grupos e funções incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="de6bd-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6bd-117">Required.</span></span> |
|<span data-ttu-id="de6bd-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="de6bd-118">clientAppTypes</span></span>|<span data-ttu-id="de6bd-119">coleção conditionalAccessClientApp</span><span class="sxs-lookup"><span data-stu-id="de6bd-119">conditionalAccessClientApp collection</span></span>| <span data-ttu-id="de6bd-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-120">Client application types included in the policy.</span></span> <span data-ttu-id="de6bd-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="de6bd-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span> <span data-ttu-id="de6bd-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6bd-122">Required.</span></span>|
|<span data-ttu-id="de6bd-123">deviceStates</span><span class="sxs-lookup"><span data-stu-id="de6bd-123">deviceStates</span></span>|[<span data-ttu-id="de6bd-124">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="de6bd-124">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="de6bd-125">Estados do dispositivo na política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-125">Device states in the policy.</span></span> |
|<span data-ttu-id="de6bd-126">devices</span><span class="sxs-lookup"><span data-stu-id="de6bd-126">devices</span></span>|[<span data-ttu-id="de6bd-127">conditionalAccessDevices</span><span class="sxs-lookup"><span data-stu-id="de6bd-127">conditionalAccessDevices</span></span>](conditionalaccessdevices.md)| <span data-ttu-id="de6bd-128">Dispositivos na política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-128">Devices in the policy.</span></span> |
|<span data-ttu-id="de6bd-129">locations</span><span class="sxs-lookup"><span data-stu-id="de6bd-129">locations</span></span>|[<span data-ttu-id="de6bd-130">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="de6bd-130">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="de6bd-131">Locais incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-131">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="de6bd-132">plataformas</span><span class="sxs-lookup"><span data-stu-id="de6bd-132">platforms</span></span>|[<span data-ttu-id="de6bd-133">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="de6bd-133">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="de6bd-134">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-134">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="de6bd-135">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="de6bd-135">signInRiskLevels</span></span>|<span data-ttu-id="de6bd-136">Coleção riskLevel</span><span class="sxs-lookup"><span data-stu-id="de6bd-136">riskLevel collection</span></span>| <span data-ttu-id="de6bd-137">Níveis de risco de login incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-137">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="de6bd-138">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="de6bd-138">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="de6bd-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6bd-139">Required.</span></span>|
|<span data-ttu-id="de6bd-140">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="de6bd-140">userRiskLevels</span></span>|<span data-ttu-id="de6bd-141">Coleção riskLevel</span><span class="sxs-lookup"><span data-stu-id="de6bd-141">riskLevel collection</span></span>| <span data-ttu-id="de6bd-142">Níveis de risco de usuário incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="de6bd-142">User risk levels included in the policy.</span></span> <span data-ttu-id="de6bd-143">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="de6bd-143">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="de6bd-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de6bd-144">Required.</span></span>|

><span data-ttu-id="de6bd-145">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="de6bd-145">**Note:**</span></span>
>* <span data-ttu-id="de6bd-146">**clientAppType** `modern` será preterido e substituído por `mobileAppsAndDesktopClients` .</span><span class="sxs-lookup"><span data-stu-id="de6bd-146">**clientAppType** `modern` is going to be deprecated and replaced by `mobileAppsAndDesktopClients`.</span></span> <br>
>* <span data-ttu-id="de6bd-147">**clientAppType** `easUnsupported` será preterido em favor do que inclui plataformas com suporte e sem suporte do `exchangeActiveSync` EAS.</span><span class="sxs-lookup"><span data-stu-id="de6bd-147">**clientAppType** `easUnsupported` is going to be deprecated in favor of `exchangeActiveSync` which includes EAS supported and unsupported platforms.</span></span> <br>
>* <span data-ttu-id="de6bd-148">Estamos preterindo a condição **deviceStates** e ela pode ser removida no futuro.</span><span class="sxs-lookup"><span data-stu-id="de6bd-148">We are deprecating the **deviceStates** condition, and it may be removed in the future.</span></span> <span data-ttu-id="de6bd-149">Em frente, use a **condição de** dispositivos.</span><span class="sxs-lookup"><span data-stu-id="de6bd-149">Going forward, use **devices** condition.</span></span>

## <a name="relationships"></a><span data-ttu-id="de6bd-150">Relações</span><span class="sxs-lookup"><span data-stu-id="de6bd-150">Relationships</span></span>

<span data-ttu-id="de6bd-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de6bd-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de6bd-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de6bd-152">JSON representation</span></span>

<span data-ttu-id="de6bd-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de6bd-153">The following is a JSON representation of the resource.</span></span>

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


