---
title: tipo de recurso privilegedRoleSummary
description: O resumo de estatísticas de uma função específica.
localization_priority: Normal
ms.openlocfilehash: 3e7b447f63c5f8545021508ae2dc137bef845210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344255"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="1d16f-103">tipo de recurso privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1d16f-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d16f-104">O resumo de estatísticas de uma função específica.</span><span class="sxs-lookup"><span data-stu-id="1d16f-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="1d16f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d16f-105">Methods</span></span>

| <span data-ttu-id="1d16f-106">Método</span><span class="sxs-lookup"><span data-stu-id="1d16f-106">Method</span></span>           | <span data-ttu-id="1d16f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d16f-107">Return Type</span></span>    |<span data-ttu-id="1d16f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d16f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1d16f-109">Get privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1d16f-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="1d16f-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="1d16f-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="1d16f-111">Leia as propriedades e os relacionamentos do objeto privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="1d16f-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1d16f-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d16f-112">Properties</span></span>
| <span data-ttu-id="1d16f-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d16f-113">Property</span></span>     | <span data-ttu-id="1d16f-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d16f-114">Type</span></span>   |<span data-ttu-id="1d16f-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d16f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d16f-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="1d16f-116">elevatedCount</span></span>|<span data-ttu-id="1d16f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="1d16f-117">int32</span></span>|<span data-ttu-id="1d16f-118">O número de usuários que têm a função atribuída e a função é ativada.</span><span class="sxs-lookup"><span data-stu-id="1d16f-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="1d16f-119">id</span><span class="sxs-lookup"><span data-stu-id="1d16f-119">id</span></span>|<span data-ttu-id="1d16f-120">string</span><span class="sxs-lookup"><span data-stu-id="1d16f-120">string</span></span>| <span data-ttu-id="1d16f-121">O identificador exclusivo da função.</span><span class="sxs-lookup"><span data-stu-id="1d16f-121">The unique identifier for the role.</span></span> <span data-ttu-id="1d16f-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1d16f-122">Read-only.</span></span>|
|<span data-ttu-id="1d16f-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="1d16f-123">managedCount</span></span>|<span data-ttu-id="1d16f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="1d16f-124">int32</span></span>|<span data-ttu-id="1d16f-125">O número de usuários que têm a função atribuída, mas a função é desativada.</span><span class="sxs-lookup"><span data-stu-id="1d16f-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="1d16f-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="1d16f-126">mfaEnabled</span></span>|<span data-ttu-id="1d16f-127">booliano</span><span class="sxs-lookup"><span data-stu-id="1d16f-127">boolean</span></span>|<span data-ttu-id="1d16f-128">**true** se a ativação de função requer MFA.</span><span class="sxs-lookup"><span data-stu-id="1d16f-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="1d16f-129">**false** se a ativação de função não requer MFA.</span><span class="sxs-lookup"><span data-stu-id="1d16f-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="1d16f-130">status</span><span class="sxs-lookup"><span data-stu-id="1d16f-130">status</span></span>|<span data-ttu-id="1d16f-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d16f-131">string</span></span>| <span data-ttu-id="1d16f-132">Os valores possíveis são: `ok` e `bad`.</span><span class="sxs-lookup"><span data-stu-id="1d16f-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="1d16f-133">O valor depende da taxa de (managedCount/usersCount).</span><span class="sxs-lookup"><span data-stu-id="1d16f-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="1d16f-134">Se a taxa for menor que um limite predefinido `ok` , será retornado.</span><span class="sxs-lookup"><span data-stu-id="1d16f-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="1d16f-135">Caso contrário `bad` , será retornado.</span><span class="sxs-lookup"><span data-stu-id="1d16f-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="1d16f-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="1d16f-136">usersCount</span></span>|<span data-ttu-id="1d16f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1d16f-137">int32</span></span>|<span data-ttu-id="1d16f-138">O número de usuários atribuídos com a função.</span><span class="sxs-lookup"><span data-stu-id="1d16f-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d16f-139">Relações</span><span class="sxs-lookup"><span data-stu-id="1d16f-139">Relationships</span></span>
<span data-ttu-id="1d16f-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d16f-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1d16f-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d16f-141">JSON representation</span></span>

<span data-ttu-id="1d16f-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d16f-142">Here is a JSON representation of the resource.</span></span>

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
