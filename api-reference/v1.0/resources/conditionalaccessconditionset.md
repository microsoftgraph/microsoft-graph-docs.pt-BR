---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ff7159c09b0afcaf223a5840584d531e99be2da6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132131"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="e48fa-103">Tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="e48fa-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="e48fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e48fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e48fa-105">Representa o tipo de condições que regem quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="e48fa-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="e48fa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e48fa-106">Properties</span></span>

| <span data-ttu-id="e48fa-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e48fa-107">Property</span></span>     | <span data-ttu-id="e48fa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e48fa-108">Type</span></span>        | <span data-ttu-id="e48fa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e48fa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e48fa-110">applications</span><span class="sxs-lookup"><span data-stu-id="e48fa-110">applications</span></span>|[<span data-ttu-id="e48fa-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="e48fa-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="e48fa-112">Aplicativos e ações do usuário incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="e48fa-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e48fa-113">Required.</span></span> |
|<span data-ttu-id="e48fa-114">usuários</span><span class="sxs-lookup"><span data-stu-id="e48fa-114">users</span></span>|[<span data-ttu-id="e48fa-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="e48fa-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="e48fa-116">Usuários, grupos e funções incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="e48fa-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e48fa-117">Required.</span></span> |
|<span data-ttu-id="e48fa-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="e48fa-118">clientAppTypes</span></span>|<span data-ttu-id="e48fa-119">String collection</span><span class="sxs-lookup"><span data-stu-id="e48fa-119">String collection</span></span>| <span data-ttu-id="e48fa-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-120">Client application types included in the policy.</span></span> <span data-ttu-id="e48fa-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="e48fa-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span>|
|<span data-ttu-id="e48fa-122">locations</span><span class="sxs-lookup"><span data-stu-id="e48fa-122">locations</span></span>|[<span data-ttu-id="e48fa-123">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="e48fa-123">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="e48fa-124">Locais incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-124">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="e48fa-125">platforms</span><span class="sxs-lookup"><span data-stu-id="e48fa-125">platforms</span></span>|[<span data-ttu-id="e48fa-126">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="e48fa-126">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="e48fa-127">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-127">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="e48fa-128">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="e48fa-128">signInRiskLevels</span></span>|<span data-ttu-id="e48fa-129">String collection</span><span class="sxs-lookup"><span data-stu-id="e48fa-129">String collection</span></span>| <span data-ttu-id="e48fa-130">Níveis de risco de login incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-130">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="e48fa-131">Os valores possíveis são: `low`, `medium`, `high`, `none`.</span><span class="sxs-lookup"><span data-stu-id="e48fa-131">Possible values are: `low`, `medium`, `high`, `none`.</span></span>|
|<span data-ttu-id="e48fa-132">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="e48fa-132">userRiskLevels</span></span>|<span data-ttu-id="e48fa-133">String collection</span><span class="sxs-lookup"><span data-stu-id="e48fa-133">String collection</span></span>| <span data-ttu-id="e48fa-134">Níveis de risco do usuário incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="e48fa-134">User risk levels included in the policy.</span></span> <span data-ttu-id="e48fa-135">Os valores possíveis são: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e48fa-135">Possible values are: `low`, `medium`, `high`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e48fa-136">Relações</span><span class="sxs-lookup"><span data-stu-id="e48fa-136">Relationships</span></span>

<span data-ttu-id="e48fa-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e48fa-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e48fa-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e48fa-138">JSON representation</span></span>

<span data-ttu-id="e48fa-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e48fa-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "clientAppTypes",
    "locations",
    "platforms",
    "signInRiskLevels",
    "userRiskLevels"
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
  "signInRiskLevels": ["String"],
  "userRiskLevels": ["String"]
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

