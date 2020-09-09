---
title: tipo de recurso expirationPattern
description: O padrão de validade em um agendamento de solicitação pode ser incluído em uma solicitação de atribuição de pacote do Access e está presente em uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62c49b7e725b923b95c514a7d3e955fed5fce46c
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413378"
---
# <a name="expirationpattern-resource-type"></a><span data-ttu-id="ecbcd-103">tipo de recurso expirationPattern</span><span class="sxs-lookup"><span data-stu-id="ecbcd-103">expirationPattern resource type</span></span>

<span data-ttu-id="ecbcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecbcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecbcd-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma solicitação de atribuição de pacote de acesso é criada por um usuário que deseja obter uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="ecbcd-106">Essa solicitação pode incluir um cronograma para quando o usuário quiser ter uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-106">This request can include a schedule for when the user would like to have an assignment.</span></span>  <span data-ttu-id="ecbcd-107">Uma atribuição de pacote do Access que resulta de tal solicitação também tem um cronograma.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-107">An access package assignment that results from such a request also has a schedule.</span></span>  <span data-ttu-id="ecbcd-108">O campo de expiração de um [requestSchedule](requestschedule.md) indica quando a atribuição de pacote de acesso deve expirar.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-108">The expiration field of a [requestSchedule](requestschedule.md) indicates when the access package assignment should expire.</span></span>

## <a name="properties"></a><span data-ttu-id="ecbcd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecbcd-109">Properties</span></span>

| <span data-ttu-id="ecbcd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecbcd-110">Property</span></span>     | <span data-ttu-id="ecbcd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecbcd-111">Type</span></span>        | <span data-ttu-id="ecbcd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecbcd-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ecbcd-113">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ecbcd-113">endDateTime</span></span>|<span data-ttu-id="ecbcd-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbcd-114">DateTimeOffset</span></span>|<span data-ttu-id="ecbcd-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ecbcd-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ecbcd-117">duration</span><span class="sxs-lookup"><span data-stu-id="ecbcd-117">duration</span></span>|<span data-ttu-id="ecbcd-118">Duração</span><span class="sxs-lookup"><span data-stu-id="ecbcd-118">Duration</span></span>|<span data-ttu-id="ecbcd-119">A duração de acesso desejada do solicitante.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-119">The requestor's desired duration of access.</span></span> <span data-ttu-id="ecbcd-120">Se especificado em uma solicitação, EndDateTime não deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-120">If specified in a request, endDateTime should not be present.</span></span>|
|<span data-ttu-id="ecbcd-121">tipo</span><span class="sxs-lookup"><span data-stu-id="ecbcd-121">type</span></span>|<span data-ttu-id="ecbcd-122">expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="ecbcd-122">expirationPatternType</span></span>|<span data-ttu-id="ecbcd-123">O tipo de padrão de expiração desejado do solicitante.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-123">The requestor's desired expiration pattern type.</span></span>|

### <a name="expirationpatterntype-values"></a><span data-ttu-id="ecbcd-124">valores de expirationPatternType</span><span class="sxs-lookup"><span data-stu-id="ecbcd-124">expirationPatternType values</span></span>

| <span data-ttu-id="ecbcd-125">Membro</span><span class="sxs-lookup"><span data-stu-id="ecbcd-125">Member</span></span> | <span data-ttu-id="ecbcd-126">Valor</span><span class="sxs-lookup"><span data-stu-id="ecbcd-126">Value</span></span>| <span data-ttu-id="ecbcd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecbcd-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ecbcd-128">Não especificado</span><span class="sxs-lookup"><span data-stu-id="ecbcd-128">notSpecified</span></span>|<span data-ttu-id="ecbcd-129">,0</span><span class="sxs-lookup"><span data-stu-id="ecbcd-129">0</span></span>|<span data-ttu-id="ecbcd-130">Nenhum cronograma de expiração especificado.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-130">No expiration schedule was specified.</span></span>|
|<span data-ttu-id="ecbcd-131">noexpiração</span><span class="sxs-lookup"><span data-stu-id="ecbcd-131">noExpiration</span></span>|<span data-ttu-id="ecbcd-132">1</span><span class="sxs-lookup"><span data-stu-id="ecbcd-132">1</span></span>|<span data-ttu-id="ecbcd-133">O solicitante não quis que o acesso expire.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-133">The requestor did not wish the access to expire.</span></span>|
|<span data-ttu-id="ecbcd-134">afterDateTime</span><span class="sxs-lookup"><span data-stu-id="ecbcd-134">afterDateTime</span></span>|<span data-ttu-id="ecbcd-135">duas</span><span class="sxs-lookup"><span data-stu-id="ecbcd-135">2</span></span>|<span data-ttu-id="ecbcd-136">O Access expirará após uma data e hora especificadas.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-136">Access will expire after a specified date and time.</span></span>|
|<span data-ttu-id="ecbcd-137">afterDuration</span><span class="sxs-lookup"><span data-stu-id="ecbcd-137">afterDuration</span></span>|<span data-ttu-id="ecbcd-138">3D</span><span class="sxs-lookup"><span data-stu-id="ecbcd-138">3</span></span>|<span data-ttu-id="ecbcd-139">O Access expirará após uma determinada duração relativa ao acesso concedido.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-139">Access will expire after a specified duration relative to access being granted.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecbcd-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecbcd-140">JSON representation</span></span>

<span data-ttu-id="ecbcd-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ecbcd-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expirationPattern",
  "baseType": ""
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
