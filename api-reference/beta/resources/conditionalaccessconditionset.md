---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dee80ebdacfda6c0b633f1aec1dd085d80eb22e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507559"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="3c4ae-103">tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="3c4ae-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="3c4ae-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3c4ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c4ae-105">Representa o tipo de condições que controlam quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="3c4ae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c4ae-106">Properties</span></span>

| <span data-ttu-id="3c4ae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c4ae-107">Property</span></span>     | <span data-ttu-id="3c4ae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c4ae-108">Type</span></span>        | <span data-ttu-id="3c4ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c4ae-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c4ae-110">Emprego</span><span class="sxs-lookup"><span data-stu-id="3c4ae-110">applications</span></span>|[<span data-ttu-id="3c4ae-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="3c4ae-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="3c4ae-112">Aplicativos e ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="3c4ae-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-113">Required.</span></span> |
|<span data-ttu-id="3c4ae-114">usuários</span><span class="sxs-lookup"><span data-stu-id="3c4ae-114">users</span></span>|[<span data-ttu-id="3c4ae-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="3c4ae-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="3c4ae-116">Usuários, grupos e funções incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="3c4ae-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-117">Required.</span></span> |
|<span data-ttu-id="3c4ae-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="3c4ae-118">clientAppTypes</span></span>|<span data-ttu-id="3c4ae-119">String collection</span><span class="sxs-lookup"><span data-stu-id="3c4ae-119">String collection</span></span>| <span data-ttu-id="3c4ae-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-120">Client application types included in the policy.</span></span> <span data-ttu-id="3c4ae-121">Os valores possíveis são: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-121">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="3c4ae-122">deviceStates</span><span class="sxs-lookup"><span data-stu-id="3c4ae-122">deviceStates</span></span>|[<span data-ttu-id="3c4ae-123">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="3c4ae-123">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="3c4ae-124">Estados do dispositivo na política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-124">Device states in the policy.</span></span> |
|<span data-ttu-id="3c4ae-125">locations</span><span class="sxs-lookup"><span data-stu-id="3c4ae-125">locations</span></span>|[<span data-ttu-id="3c4ae-126">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="3c4ae-126">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="3c4ae-127">Locais incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-127">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="3c4ae-128">plataformas</span><span class="sxs-lookup"><span data-stu-id="3c4ae-128">platforms</span></span>|[<span data-ttu-id="3c4ae-129">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="3c4ae-129">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="3c4ae-130">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-130">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="3c4ae-131">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="3c4ae-131">signInRiskLevels</span></span>|<span data-ttu-id="3c4ae-132">String collection</span><span class="sxs-lookup"><span data-stu-id="3c4ae-132">String collection</span></span>| <span data-ttu-id="3c4ae-133">Níveis de risco incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-133">Risk levels included in the policy.</span></span> <span data-ttu-id="3c4ae-134">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-134">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c4ae-135">Relações</span><span class="sxs-lookup"><span data-stu-id="3c4ae-135">Relationships</span></span>

<span data-ttu-id="3c4ae-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c4ae-136">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c4ae-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c4ae-137">JSON representation</span></span>

<span data-ttu-id="3c4ae-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c4ae-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "deviceStates",
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