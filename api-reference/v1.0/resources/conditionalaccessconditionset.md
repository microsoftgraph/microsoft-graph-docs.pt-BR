---
title: Tipo de recurso conditionalAccessConditionSet
description: Representa o tipo de condições que regem quando a política se aplica.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3d448b2d54fbc94c63588712f06492ce7d38a33a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962494"
---
# <a name="conditionalaccessconditionset-resource-type"></a><span data-ttu-id="78321-103">Tipo de recurso conditionalAccessConditionSet</span><span class="sxs-lookup"><span data-stu-id="78321-103">conditionalAccessConditionSet resource type</span></span>

<span data-ttu-id="78321-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78321-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78321-105">Representa o tipo de condições que regem quando a política se aplica.</span><span class="sxs-lookup"><span data-stu-id="78321-105">Represents the type of conditions that govern when the policy applies.</span></span>

## <a name="properties"></a><span data-ttu-id="78321-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78321-106">Properties</span></span>

| <span data-ttu-id="78321-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78321-107">Property</span></span>     | <span data-ttu-id="78321-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="78321-108">Type</span></span>        | <span data-ttu-id="78321-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="78321-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78321-110">applications</span><span class="sxs-lookup"><span data-stu-id="78321-110">applications</span></span>|[<span data-ttu-id="78321-111">conditionalAccessApplications</span><span class="sxs-lookup"><span data-stu-id="78321-111">conditionalAccessApplications</span></span>](conditionalaccessapplications.md)| <span data-ttu-id="78321-112">Aplicativos e ações do usuário incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="78321-112">Applications and user actions included in and excluded from the policy.</span></span> <span data-ttu-id="78321-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78321-113">Required.</span></span> |
|<span data-ttu-id="78321-114">usuários</span><span class="sxs-lookup"><span data-stu-id="78321-114">users</span></span>|[<span data-ttu-id="78321-115">conditionalAccessUsers</span><span class="sxs-lookup"><span data-stu-id="78321-115">conditionalAccessUsers</span></span>](conditionalaccessusers.md)| <span data-ttu-id="78321-116">Usuários, grupos e funções incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="78321-116">Users, groups, and roles included in and excluded from the policy.</span></span> <span data-ttu-id="78321-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78321-117">Required.</span></span> |
|<span data-ttu-id="78321-118">clientAppTypes</span><span class="sxs-lookup"><span data-stu-id="78321-118">clientAppTypes</span></span>|<span data-ttu-id="78321-119">coleção conditionalAccessClientApp</span><span class="sxs-lookup"><span data-stu-id="78321-119">conditionalAccessClientApp collection</span></span>| <span data-ttu-id="78321-120">Tipos de aplicativo cliente incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="78321-120">Client application types included in the policy.</span></span> <span data-ttu-id="78321-121">Os possíveis valores são: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span><span class="sxs-lookup"><span data-stu-id="78321-121">Possible values are: `all`, `browser`, `mobileAppsAndDesktopClients`, `exchangeActiveSync`, `easSupported`, `other`.</span></span> <span data-ttu-id="78321-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78321-122">Required.</span></span>|
|<span data-ttu-id="78321-123">locations</span><span class="sxs-lookup"><span data-stu-id="78321-123">locations</span></span>|[<span data-ttu-id="78321-124">conditionalAccessLocations</span><span class="sxs-lookup"><span data-stu-id="78321-124">conditionalAccessLocations</span></span>](conditionalaccesslocations.md)| <span data-ttu-id="78321-125">Locais incluídos e excluídos da política.</span><span class="sxs-lookup"><span data-stu-id="78321-125">Locations included in and excluded from the policy.</span></span> |
|<span data-ttu-id="78321-126">plataformas</span><span class="sxs-lookup"><span data-stu-id="78321-126">platforms</span></span>|[<span data-ttu-id="78321-127">conditionalAccessPlatforms</span><span class="sxs-lookup"><span data-stu-id="78321-127">conditionalAccessPlatforms</span></span>](conditionalaccessplatforms.md)| <span data-ttu-id="78321-128">Plataformas incluídas e excluídas da política.</span><span class="sxs-lookup"><span data-stu-id="78321-128">Platforms included in and excluded from the policy.</span></span> |
|<span data-ttu-id="78321-129">signInRiskLevels</span><span class="sxs-lookup"><span data-stu-id="78321-129">signInRiskLevels</span></span>|<span data-ttu-id="78321-130">Coleção riskLevel</span><span class="sxs-lookup"><span data-stu-id="78321-130">riskLevel collection</span></span>| <span data-ttu-id="78321-131">Níveis de risco de login incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="78321-131">Sign-in risk levels included in the policy.</span></span> <span data-ttu-id="78321-132">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="78321-132">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="78321-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78321-133">Required.</span></span>|
|<span data-ttu-id="78321-134">userRiskLevels</span><span class="sxs-lookup"><span data-stu-id="78321-134">userRiskLevels</span></span>|<span data-ttu-id="78321-135">Coleção riskLevel</span><span class="sxs-lookup"><span data-stu-id="78321-135">riskLevel collection</span></span>| <span data-ttu-id="78321-136">Níveis de risco de usuário incluídos na política.</span><span class="sxs-lookup"><span data-stu-id="78321-136">User risk levels included in the policy.</span></span> <span data-ttu-id="78321-137">Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="78321-137">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="78321-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78321-138">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78321-139">Relações</span><span class="sxs-lookup"><span data-stu-id="78321-139">Relationships</span></span>

<span data-ttu-id="78321-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78321-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78321-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78321-141">JSON representation</span></span>

<span data-ttu-id="78321-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78321-142">The following is a JSON representation of the resource.</span></span>

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

