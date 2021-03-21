---
title: Tipo de recurso privilegedRoleSummary
description: O resumo de estatísticas para uma função específica.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 962cd1b830542c5b17c5f742af357d5855b81886
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962557"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="73f61-103">Tipo de recurso privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="73f61-103">privilegedRoleSummary resource type</span></span>

<span data-ttu-id="73f61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73f61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f61-105">O resumo de estatísticas para uma função específica.</span><span class="sxs-lookup"><span data-stu-id="73f61-105">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="73f61-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="73f61-106">Methods</span></span>

| <span data-ttu-id="73f61-107">Método</span><span class="sxs-lookup"><span data-stu-id="73f61-107">Method</span></span>           | <span data-ttu-id="73f61-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73f61-108">Return Type</span></span>    |<span data-ttu-id="73f61-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73f61-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73f61-110">Get privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="73f61-110">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="73f61-111">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="73f61-111">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="73f61-112">Ler propriedades e relações do objeto privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="73f61-112">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73f61-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73f61-113">Properties</span></span>
| <span data-ttu-id="73f61-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73f61-114">Property</span></span>     | <span data-ttu-id="73f61-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="73f61-115">Type</span></span>   |<span data-ttu-id="73f61-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="73f61-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73f61-117">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="73f61-117">elevatedCount</span></span>|<span data-ttu-id="73f61-118">int32</span><span class="sxs-lookup"><span data-stu-id="73f61-118">int32</span></span>|<span data-ttu-id="73f61-119">O número de usuários que têm a função atribuída e a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="73f61-119">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="73f61-120">id</span><span class="sxs-lookup"><span data-stu-id="73f61-120">id</span></span>|<span data-ttu-id="73f61-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73f61-121">string</span></span>| <span data-ttu-id="73f61-122">O identificador exclusivo da função.</span><span class="sxs-lookup"><span data-stu-id="73f61-122">The unique identifier for the role.</span></span> <span data-ttu-id="73f61-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73f61-123">Read-only.</span></span>|
|<span data-ttu-id="73f61-124">managedCount</span><span class="sxs-lookup"><span data-stu-id="73f61-124">managedCount</span></span>|<span data-ttu-id="73f61-125">int32</span><span class="sxs-lookup"><span data-stu-id="73f61-125">int32</span></span>|<span data-ttu-id="73f61-126">O número de usuários que têm a função atribuída, mas a função é desativada.</span><span class="sxs-lookup"><span data-stu-id="73f61-126">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="73f61-127">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="73f61-127">mfaEnabled</span></span>|<span data-ttu-id="73f61-128">booliano</span><span class="sxs-lookup"><span data-stu-id="73f61-128">boolean</span></span>|<span data-ttu-id="73f61-129">`true` se a ativação de função exigir MFA.</span><span class="sxs-lookup"><span data-stu-id="73f61-129">`true` if the role activation requires MFA.</span></span> <span data-ttu-id="73f61-130">`false` se a ativação de função não exigir MFA.</span><span class="sxs-lookup"><span data-stu-id="73f61-130">`false` if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="73f61-131">status</span><span class="sxs-lookup"><span data-stu-id="73f61-131">status</span></span>|<span data-ttu-id="73f61-132">roleSummaryStatus</span><span class="sxs-lookup"><span data-stu-id="73f61-132">roleSummaryStatus</span></span>| <span data-ttu-id="73f61-133">Os valores possíveis são: `ok` e `bad`.</span><span class="sxs-lookup"><span data-stu-id="73f61-133">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="73f61-134">O valor depende da taxa de (managedCount /usersCount).</span><span class="sxs-lookup"><span data-stu-id="73f61-134">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="73f61-135">Se a taxa for menor que um limite predefinido, `ok` será retornado.</span><span class="sxs-lookup"><span data-stu-id="73f61-135">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="73f61-136">Caso contrário, `bad` será retornado.</span><span class="sxs-lookup"><span data-stu-id="73f61-136">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="73f61-137">usersCount</span><span class="sxs-lookup"><span data-stu-id="73f61-137">usersCount</span></span>|<span data-ttu-id="73f61-138">int32</span><span class="sxs-lookup"><span data-stu-id="73f61-138">int32</span></span>|<span data-ttu-id="73f61-139">O número de usuários atribuídos à função.</span><span class="sxs-lookup"><span data-stu-id="73f61-139">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73f61-140">Relações</span><span class="sxs-lookup"><span data-stu-id="73f61-140">Relationships</span></span>
<span data-ttu-id="73f61-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73f61-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="73f61-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73f61-142">JSON representation</span></span>

<span data-ttu-id="73f61-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73f61-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


