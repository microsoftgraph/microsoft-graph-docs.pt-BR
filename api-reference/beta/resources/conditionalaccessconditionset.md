---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e81e8b2748a7dc3b6a9ca028472c1f6ab153b0e
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638509"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="db27d-103">tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="db27d-103">conditionalAccessConditionSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db27d-104">Representa o tipo de condições que controlam quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="db27d-104">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="db27d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db27d-105">Properties</span></span>

| <span data-ttu-id="db27d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db27d-106">Property</span></span>     | <span data-ttu-id="db27d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="db27d-107">Type</span></span>        | <span data-ttu-id="db27d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="db27d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="db27d-109">Emprego</span><span class="sxs-lookup"><span data-stu-id="db27d-109">applications</span></span>|[<span data-ttu-id="db27d-110">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="db27d-110">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="db27d-111">Aplicativos e ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="db27d-111">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="db27d-112">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db27d-112">Required.</span></span> |
|<span data-ttu-id="db27d-113">usuários</span><span class="sxs-lookup"><span data-stu-id="db27d-113">users</span></span>|[<span data-ttu-id="db27d-114">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="db27d-114">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="db27d-115">Usuários, grupos e funções incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="db27d-115">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="db27d-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db27d-116">Required.</span></span> |
|<span data-ttu-id="db27d-117">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="db27d-117">clientAppTypes</span></span>|<span data-ttu-id="db27d-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db27d-118">String collection</span></span>| <span data-ttu-id="db27d-119">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="db27d-119">Client application types included in the policy.</span></span> <span data-ttu-id="db27d-120">Os valores possíveis são: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="db27d-120">Possible values are: `browser`, `modern`, `easSupported`, `easUnsupported`, `other`.</span></span>|
|<span data-ttu-id="db27d-121">deviceStates</span><span class="sxs-lookup"><span data-stu-id="db27d-121">deviceStates</span></span>|[<span data-ttu-id="db27d-122">conditionalAccessDeviceStates</span><span class="sxs-lookup"><span data-stu-id="db27d-122">conditionalAccessDeviceStates</span></span>](conditionalaccessdevicestates.md)| <span data-ttu-id="db27d-123">Estados do dispositivo na política.</span><span class="sxs-lookup"><span data-stu-id="db27d-123">Device states in the policy.</span></span> |
|<span data-ttu-id="db27d-124">locations</span><span class="sxs-lookup"><span data-stu-id="db27d-124">locations</span></span>|[<span data-ttu-id="db27d-125">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="db27d-125">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="db27d-126">Locais incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="db27d-126">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="db27d-127">plataformas</span><span class="sxs-lookup"><span data-stu-id="db27d-127">platforms</span></span>|[<span data-ttu-id="db27d-128">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="db27d-128">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="db27d-129">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="db27d-129">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="db27d-130">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="db27d-130">signInRiskLevels</span></span>|<span data-ttu-id="db27d-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db27d-131">String collection</span></span>| <span data-ttu-id="db27d-132">Níveis de risco incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="db27d-132">Risk levels included in the policy.</span></span> <span data-ttu-id="db27d-133">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="db27d-133">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db27d-134">Relações</span><span class="sxs-lookup"><span data-stu-id="db27d-134">Relationships</span></span>

<span data-ttu-id="db27d-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db27d-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db27d-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db27d-136">JSON representation</span></span>

<span data-ttu-id="db27d-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db27d-137">The following is a JSON representation of the resource.</span></span>

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