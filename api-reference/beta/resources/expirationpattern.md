---
title: Tipo de recurso expirationPattern
description: O padrão de expiração em um cronograma de solicitação pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b6587d8ba410ba0240c0fd75b7c8ec37105061d8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721289"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="21370-103">Tipo de recurso expirationPattern</span><span class="sxs-lookup"><span data-stu-id="21370-103">expirationPattern resource type</span></span>

<span data-ttu-id="21370-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21370-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21370-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="21370-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="21370-106">Essa solicitação pode incluir um cronograma para quando o usuário gostaria de ter uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="21370-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="21370-107">Uma atribuição de pacote de acesso que resulta de tal solicitação também tem um cronograma.</span><span class="sxs-lookup"><span data-stu-id="21370-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="21370-108">O campo de expiração de [um requestSchedule](requestschedule.md) indica quando a atribuição do pacote de acesso deve expirar.</span><span class="sxs-lookup"><span data-stu-id="21370-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="21370-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21370-109">Properties</span></span>

| <span data-ttu-id="21370-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21370-110">Property</span></span>     | <span data-ttu-id="21370-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="21370-111">Type</span></span>        | <span data-ttu-id="21370-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="21370-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21370-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="21370-113">endDateTime</span></span>|<span data-ttu-id="21370-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21370-114">DateTimeOffset</span></span>|<span data-ttu-id="21370-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="21370-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="21370-116">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="21370-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="21370-117">duração</span><span class="sxs-lookup"><span data-stu-id="21370-117">duration</span></span>|<span data-ttu-id="21370-118">Duration</span><span class="sxs-lookup"><span data-stu-id="21370-118">Duration</span></span>|<span data-ttu-id="21370-119">A duração desejada do acesso do solicitante.</span><span class="sxs-lookup"><span data-stu-id="21370-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="21370-120">Se especificado em uma solicitação, endDateTime não deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="21370-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="21370-121">tipo</span><span class="sxs-lookup"><span data-stu-id="21370-121">type</span></span>|<span data-ttu-id="21370-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="21370-122">expirationPatternType</span></span>|<span data-ttu-id="21370-123">O tipo de padrão de expiração desejado do solicitante.</span><span class="sxs-lookup"><span data-stu-id="21370-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="21370-124">valores expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="21370-124">expirationPatternType values</span></span>

| <span data-ttu-id="21370-125">Membro</span><span class="sxs-lookup"><span data-stu-id="21370-125">Member</span></span> | <span data-ttu-id="21370-126">Valor</span><span class="sxs-lookup"><span data-stu-id="21370-126">Value</span></span>| <span data-ttu-id="21370-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="21370-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="21370-128">notSpecified</span><span class="sxs-lookup"><span data-stu-id="21370-128">notSpecified</span></span>|<span data-ttu-id="21370-129">0</span><span class="sxs-lookup"><span data-stu-id="21370-129">0</span></span>|<span data-ttu-id="21370-130">Nenhum cronograma de expiração foi especificado.</span><span class="sxs-lookup"><span data-stu-id="21370-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="21370-131">noExpiration</span><span class="sxs-lookup"><span data-stu-id="21370-131">noExpiration</span></span>|<span data-ttu-id="21370-132">1</span><span class="sxs-lookup"><span data-stu-id="21370-132">1</span></span>|<span data-ttu-id="21370-133">O solicitante não desejou que o acesso expirar.</span><span class="sxs-lookup"><span data-stu-id="21370-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="21370-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="21370-134">afterDateTime</span></span>|<span data-ttu-id="21370-135">2 </span><span class="sxs-lookup"><span data-stu-id="21370-135">2</span></span>|<span data-ttu-id="21370-136">O acesso expirará após uma data e hora especificadas.</span><span class="sxs-lookup"><span data-stu-id="21370-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="21370-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="21370-137">afterDuration</span></span>|<span data-ttu-id="21370-138">3 </span><span class="sxs-lookup"><span data-stu-id="21370-138">3</span></span>|<span data-ttu-id="21370-139">O acesso expirará após uma duração especificada relativa ao acesso que está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="21370-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21370-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21370-140">JSON representation</span></span>

<span data-ttu-id="21370-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21370-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern"
}-->

```json
{
    "endDateTime": "2020-09-10T23:06:53.307Z",
    "type": "afterDateTime"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expirationPattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


