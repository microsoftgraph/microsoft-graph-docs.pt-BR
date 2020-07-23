---
title: tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que controlam quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 993201181a9256b54663ce279c914e3669f4dc91
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384408"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="858e8-103">tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="858e8-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="858e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="858e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="858e8-105">Representa o tipo de condições que controlam quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="858e8-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="858e8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="858e8-106">Properties</span></span>

| <span data-ttu-id="858e8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="858e8-107">Property</span></span>     | <span data-ttu-id="858e8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="858e8-108">Type</span></span>        | <span data-ttu-id="858e8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="858e8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="858e8-110">Emprego</span><span class="sxs-lookup"><span data-stu-id="858e8-110">applications</span></span>|[<span data-ttu-id="858e8-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="858e8-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="858e8-112">Aplicativos e ações do usuário incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="858e8-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="858e8-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="858e8-113">Required.</span></span> |
|<span data-ttu-id="858e8-114">usuários</span><span class="sxs-lookup"><span data-stu-id="858e8-114">users</span></span>|[<span data-ttu-id="858e8-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="858e8-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="858e8-116">Usuários, grupos e funções incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="858e8-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="858e8-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="858e8-117">Required.</span></span> |
|<span data-ttu-id="858e8-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="858e8-118">clientAppTypes</span></span>|<span data-ttu-id="858e8-119">String collection</span><span class="sxs-lookup"><span data-stu-id="858e8-119">String collection</span></span>| <span data-ttu-id="858e8-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="858e8-120">Client application types included in the policy.</span></span> <span data-ttu-id="858e8-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="858e8-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="858e8-122">locations</span><span class="sxs-lookup"><span data-stu-id="858e8-122">locations</span></span>|[<span data-ttu-id="858e8-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="858e8-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="858e8-124">Locais incluídos no e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="858e8-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="858e8-125">plataformas</span><span class="sxs-lookup"><span data-stu-id="858e8-125">platforms</span></span>|[<span data-ttu-id="858e8-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="858e8-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="858e8-127">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="858e8-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="858e8-128">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="858e8-128">signInRiskLevels</span></span>|<span data-ttu-id="858e8-129">String collection</span><span class="sxs-lookup"><span data-stu-id="858e8-129">String collection</span></span>| <span data-ttu-id="858e8-130">Níveis de risco incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="858e8-130">Risk levels included in the policy.</span></span> <span data-ttu-id="858e8-131">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="858e8-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="858e8-132">Relações</span><span class="sxs-lookup"><span data-stu-id="858e8-132">Relationships</span></span>

<span data-ttu-id="858e8-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="858e8-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="858e8-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="858e8-134">JSON representation</span></span>

<span data-ttu-id="858e8-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="858e8-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
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
  "locations": {"@odata.type": "microsoft.graph.conditionalAccessLocations"},
  "platforms": {"@odata.type": "microsoft.graph.conditionalAccessPlatforms"},
  "signInRiskLevels": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessConditionSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
