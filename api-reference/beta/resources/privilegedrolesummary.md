---
title: tipo de recurso de privilegedRoleSummary
description: As estatísticas de resumida de uma determinada função.
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513736"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="b2913-103">tipo de recurso de privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="b2913-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2913-104">As estatísticas de resumida de uma determinada função.</span><span class="sxs-lookup"><span data-stu-id="b2913-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="b2913-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b2913-105">Methods</span></span>

| <span data-ttu-id="b2913-106">Método</span><span class="sxs-lookup"><span data-stu-id="b2913-106">Method</span></span>           | <span data-ttu-id="b2913-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b2913-107">Return Type</span></span>    |<span data-ttu-id="b2913-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2913-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b2913-109">Obter privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="b2913-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="b2913-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="b2913-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="b2913-111">Leia as propriedades e os relacionamentos do objeto privilegedRoleSummary.</span><span class="sxs-lookup"><span data-stu-id="b2913-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2913-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2913-112">Properties</span></span>
| <span data-ttu-id="b2913-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2913-113">Property</span></span>     | <span data-ttu-id="b2913-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2913-114">Type</span></span>   |<span data-ttu-id="b2913-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2913-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2913-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="b2913-116">elevatedCount</span></span>|<span data-ttu-id="b2913-117">int32</span><span class="sxs-lookup"><span data-stu-id="b2913-117">int32</span></span>|<span data-ttu-id="b2913-118">O número de usuários que possuem a função atribuída e a função está ativado.</span><span class="sxs-lookup"><span data-stu-id="b2913-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="b2913-119">id</span><span class="sxs-lookup"><span data-stu-id="b2913-119">id</span></span>|<span data-ttu-id="b2913-120">string</span><span class="sxs-lookup"><span data-stu-id="b2913-120">string</span></span>| <span data-ttu-id="b2913-121">O identificador exclusivo para a função.</span><span class="sxs-lookup"><span data-stu-id="b2913-121">The unique identifier for the role.</span></span> <span data-ttu-id="b2913-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2913-122">Read-only.</span></span>|
|<span data-ttu-id="b2913-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="b2913-123">managedCount</span></span>|<span data-ttu-id="b2913-124">int32</span><span class="sxs-lookup"><span data-stu-id="b2913-124">int32</span></span>|<span data-ttu-id="b2913-125">O número de usuários que possuem a função atribuída, mas a função é desativado.</span><span class="sxs-lookup"><span data-stu-id="b2913-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="b2913-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="b2913-126">mfaEnabled</span></span>|<span data-ttu-id="b2913-127">booliano</span><span class="sxs-lookup"><span data-stu-id="b2913-127">boolean</span></span>|<span data-ttu-id="b2913-128">**true** se a ativação de função requer MFA.</span><span class="sxs-lookup"><span data-stu-id="b2913-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="b2913-129">**false** se a ativação de função não exige MFA.</span><span class="sxs-lookup"><span data-stu-id="b2913-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="b2913-130">status</span><span class="sxs-lookup"><span data-stu-id="b2913-130">status</span></span>|<span data-ttu-id="b2913-131">string</span><span class="sxs-lookup"><span data-stu-id="b2913-131">string</span></span>| <span data-ttu-id="b2913-132">Os valores possíveis são: `ok` e `bad`.</span><span class="sxs-lookup"><span data-stu-id="b2913-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="b2913-133">O valor depende a proporção entre (managedCount / usersCount).</span><span class="sxs-lookup"><span data-stu-id="b2913-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="b2913-134">Se a taxa for menor que um limite predefinido, `ok` é retornado.</span><span class="sxs-lookup"><span data-stu-id="b2913-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="b2913-135">Caso contrário, `bad` é retornado.</span><span class="sxs-lookup"><span data-stu-id="b2913-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="b2913-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="b2913-136">usersCount</span></span>|<span data-ttu-id="b2913-137">int32</span><span class="sxs-lookup"><span data-stu-id="b2913-137">int32</span></span>|<span data-ttu-id="b2913-138">O número de usuários que são atribuídos com a função.</span><span class="sxs-lookup"><span data-stu-id="b2913-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2913-139">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="b2913-139">Relationships</span></span>
<span data-ttu-id="b2913-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2913-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b2913-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2913-141">JSON representation</span></span>

<span data-ttu-id="b2913-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b2913-142">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
