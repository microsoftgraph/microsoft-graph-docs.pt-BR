---
title: Tipo de recurso expirationPattern
description: O padrão de expiração em um cronograma de solicitação pode ser incluído em uma solicitação de atribuição de pacote de acesso e está presente em uma atribuição de pacote de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 250c01172e44d8ea5f3cdea94a9ac61a89a11c1b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761406"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="55818-103">Tipo de recurso expirationPattern</span><span class="sxs-lookup"><span data-stu-id="55818-103">expirationPattern resource type</span></span>

<span data-ttu-id="55818-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55818-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55818-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="55818-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="55818-106">Essa solicitação pode incluir um cronograma para quando o usuário gostaria de ter uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="55818-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="55818-107">Uma atribuição de pacote de acesso que resulta de tal solicitação também tem um cronograma.</span><span class="sxs-lookup"><span data-stu-id="55818-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="55818-108">O campo de expiração de [um requestSchedule](requestschedule.md) indica quando a atribuição do pacote de acesso deve expirar.</span><span class="sxs-lookup"><span data-stu-id="55818-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="55818-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55818-109">Properties</span></span>

| <span data-ttu-id="55818-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55818-110">Property</span></span>     | <span data-ttu-id="55818-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="55818-111">Type</span></span>        | <span data-ttu-id="55818-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="55818-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55818-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="55818-113">endDateTime</span></span>|<span data-ttu-id="55818-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55818-114">DateTimeOffset</span></span>|<span data-ttu-id="55818-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="55818-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55818-116">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="55818-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="55818-117">duração</span><span class="sxs-lookup"><span data-stu-id="55818-117">duration</span></span>|<span data-ttu-id="55818-118">Duration</span><span class="sxs-lookup"><span data-stu-id="55818-118">Duration</span></span>|<span data-ttu-id="55818-119">A duração desejada do acesso do solicitante.</span><span class="sxs-lookup"><span data-stu-id="55818-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="55818-120">Se especificado em uma solicitação, endDateTime não deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="55818-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="55818-121">tipo</span><span class="sxs-lookup"><span data-stu-id="55818-121">type</span></span>|<span data-ttu-id="55818-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="55818-122">expirationPatternType</span></span>|<span data-ttu-id="55818-123">O tipo de padrão de expiração desejado do solicitante.</span><span class="sxs-lookup"><span data-stu-id="55818-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="55818-124">valores expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="55818-124">expirationPatternType values</span></span>

| <span data-ttu-id="55818-125">Membro</span><span class="sxs-lookup"><span data-stu-id="55818-125">Member</span></span> | <span data-ttu-id="55818-126">Valor</span><span class="sxs-lookup"><span data-stu-id="55818-126">Value</span></span>| <span data-ttu-id="55818-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="55818-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="55818-128">notSpecified</span><span class="sxs-lookup"><span data-stu-id="55818-128">notSpecified</span></span>|<span data-ttu-id="55818-129">0</span><span class="sxs-lookup"><span data-stu-id="55818-129">0</span></span>|<span data-ttu-id="55818-130">Nenhum cronograma de expiração foi especificado.</span><span class="sxs-lookup"><span data-stu-id="55818-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="55818-131">noExpiration</span><span class="sxs-lookup"><span data-stu-id="55818-131">noExpiration</span></span>|<span data-ttu-id="55818-132">1</span><span class="sxs-lookup"><span data-stu-id="55818-132">1</span></span>|<span data-ttu-id="55818-133">O solicitante não desejou que o acesso expirar.</span><span class="sxs-lookup"><span data-stu-id="55818-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="55818-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="55818-134">afterDateTime</span></span>|<span data-ttu-id="55818-135">2</span><span class="sxs-lookup"><span data-stu-id="55818-135">2</span></span>|<span data-ttu-id="55818-136">O acesso expirará após uma data e hora especificadas.</span><span class="sxs-lookup"><span data-stu-id="55818-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="55818-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="55818-137">afterDuration</span></span>|<span data-ttu-id="55818-138">3</span><span class="sxs-lookup"><span data-stu-id="55818-138">3</span></span>|<span data-ttu-id="55818-139">O acesso expirará após uma duração especificada relativa ao acesso que está sendo concedido.</span><span class="sxs-lookup"><span data-stu-id="55818-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55818-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55818-140">JSON representation</span></span>

<span data-ttu-id="55818-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55818-141">The following is a JSON representation of the resource.</span></span>

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


